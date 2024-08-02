# JSON Element Explanation

## Personal Information

### Example JSON Element
```json
{
  "personal_info": {
    "coverage_amount": "5000",
    "premium_amount": null,
    "coverage_type": "Level",
    "sex": "Female",
    "state": "California",
    "month": "6",
    "day": "15",
    "year": "1980",
    "feet": "5",
    "inches": "6",
    "pounds": "140",
    "nicotine_use": "None",
    "payment_type": "Credit Card",
    "callSID": "CAabcdef123456abcdef1234567890abcd",  // YOU must inform this
    "phone": "(602) 123-4567"  // You must inform this
  }
}
```

### Detailed Explanation

#### Coverage and Premium Amounts
- If both `coverage_amount` and `premium_amount` are provided:
  ```json
  "coverage_amount": "5000",
  "premium_amount": "250"
  ```
  Only `premium_amount` will be considered.

- If only `premium_amount` is provided:
  ```json
  "coverage_amount": null,
  "premium_amount": "250"
  ```
  `premium_amount` will be considered.

- If only `coverage_amount` is provided:
  ```json
  "coverage_amount": "5000",
  "premium_amount": null
  ```
  `coverage_amount` will be considered.

- If both `coverage_amount` and `premium_amount` are null:
  ```json
  "coverage_amount": null,
  "premium_amount": null
  ```
  The system will throw an exception and end the operation for your fixing.

#### Coverage Type
The type of insurance coverage can be one of the following:
- `"Level"`
- `"Graded/Modified"`
- `"Guaranteed"`
- `"Limited Pay"`

#### Sex
The sex of the individual can be one of the following:
- `"Male"`
- `"Female"`

#### State
The state of residence can be any of the 50 US states.

#### Birthday
The birthdate of the individual, broken down into:
- `"month"`: A number from `"1"` to `"12"` representing the month of birth.
- `"day"`: A number from `"1"` to `"31"` representing the day of birth.
- `"year"`: A four-digit year representing the year of birth, e.g., `"1980"`.

#### Height/Weight
The height and weight of the individual, represented by:
- `"feet"`: The number of feet in height, e.g., `"5"`.
- `"inches"`: The number of inches in height, e.g., `"6"`.
- `"pounds"`: The weight in pounds, e.g., `"140"`.

#### Nicotine Use
The nicotine use status of the individual, which can be one of the following:
- `"None"`
- `"Cigarettes"`
- `"Cigarettes + Other Nicotine Products"`
- `"Occasional pipe/cigar use only"`
- `"Other Nicotine Products"`

#### Payment Type
The preferred payment method, which can be one of the following:
- `"Bank Draft/EFT"`
- `"Direct Express"`
- `"Credit Card"`
- `"Debit Card"`

### Required Fields
- `"callSID": "CAabcdef123456abcdef1234567890abcd"`: You must inform this.
- `"phone": "(602) 123-4567"`: You must inform this.

### Note on Number Types
- `coverage_amount` and `premium_amount` can be integers or numbers as strings.
- All other fields that represent numbers can also be integers or numbers as strings.

### Health Conditions and Medications
Each health condition and medication has its own specific set of fields and requirements. Detailed documentation about the JSON schema for each medication and health condition will be provided separately to assist in the construction and submission of these elements. Please refer to the respective documentation for more information on how to structure and fill in the JSON elements for specific health conditions and medications.

### Submission URL
To post the JSON element, use the following URL:  
[https://itkbot.bravog.com/upload-config](https://itkbot.bravog.com/upload-config)

### Example of 5 Quotation Requests
```json
[
  {
    "personal_info": {
      "coverage_amount": null,
      "premium_amount": "170",
      "coverage_type": "Level",
      "sex": "Female",
      "state": "California",
      "month": "6",
      "day": "15",
      "year": "1980",
      "feet": "5",
      "inches": "6",
      "pounds": "140",
      "nicotine_use": "None",
      "payment_type": "Credit Card",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {
      "Alcohol abuse": {
        "Date of last treatment": {
          "month": "Jun",
          "day": "18",
          "year": "2023"
        },
        "narcotics_abuse": "Yes"
      },
      "Diabetes": {
        "Date of last treatment": {
          "month": "Mar",
          "day": "14",
          "year": "2023"
        },
        "Date of diagnosis?": {
          "month": "Nov",
          "day": "22",
          "year": "2019"
        },
        "insulin_use": "No",
        "age_insulin_started": "14",
        "daily_insulin_units": "25 units",
        "uncontrolled_diabetes_past_10_years": "No",
        "uncontrolled_diabetes_past_3_years": "No",
        "uncontrolled_diabetes_past_2_years": "No",
        "uncontrolled_diabetes_past_year": "Yes",
        "changes_in_medications_past_year": "No",
        "taking_3_or_more_medications": "Yes",
        "a1c_reading_less_than_8": "Yes",
        "a1c_reading_between_8_8_6": "No",
        "a1c_reading_between_8_7_9_9": "No",
        "a1c_reading_between_10_11": "No"
      },
      "Heart attack": {
        "Date of occurrence": {
          "month": "Aug",
          "day": "5",
          "year": "2022"
        },
        "multiple_heart_attacks": "Yes"
      }
    },
    "drugs": {
      "Plavix": {
        "indication": "Atrial Fibrillation (AFIB)",
        "last_use_date": {
          "month": "May",
          "day": "7",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Jul",
          "day": "19",
          "year": "2023"
        },
        "dosage_over_75mg": "Yes",
        "episode_afib_last_12_months": "Yes"
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": "13000",
      "premium_amount": null,
      "coverage_type": "Level",
      "sex": "Male",
      "state": "Texas",
      "month": "7",
      "day": "20",
      "year": "1965",
      "feet": "6",
      "inches": "0",
      "pounds": "185",
      "nicotine_use": "Cigarettes",
      "payment_type": "Bank Draft/EFT",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {},
    "drugs": {
      "Valium": {
        "indication": "Seizures",
        "last_use_date": {
          "month": "Jun",
          "day": "10",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Aug",
          "day": "15",
          "year": "2023"
        },
        "Date of last seizure": {
          "month": "May",
          "day": "5",
          "year": "2024"
        },
        "seizures_past_2_years": "Yes",
        "more_than_1_seizure_past_year": "Yes",
        "more_than_6_seizures_past_year": "Yes",
        "more_than_12_seizures_past_3_years": "Yes",
        "condition_well_controlled": "Yes",
        "grand_mal_epilepsy": "Yes"
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": "11000",
      "premium_amount": "250",
      "coverage_type": "Level",
      "sex": "Female",
      "state": "Florida",
      "month": "9",
      "day": "13",
      "year": "1982",
      "feet": "5",
      "inches": "3",
      "pounds": "130",
      "nicotine_use": "None",
      "payment_type": "Credit Card",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone":

 "(602) 123-4567"
    },
    "health_conditions": {
      "Diabetic neuropathy": {
        "Date of last treatment": {
          "month": "Oct",
          "day": "4",
          "year": "2021"
        },
        "Date of diagnosis?": {
          "month": "Feb",
          "day": "18",
          "year": "2018"
        },
        "insulin_use": "No",
        "uncontrolled_diabetes_2_years": "Yes",
        "a1c_reading_less_than_8": "No",
        "a1c_reading_between_8_8_6": "Yes",
        "a1c_reading_between_8_7_9_9": "No"
      }
    },
    "drugs": {
      "Celebrex": {
        "indication": "Rheumatoid Arthritis",
        "last_use_date": {
          "month": "Apr",
          "day": "15",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "May",
          "day": "11",
          "year": "2023"
        }
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": null,
      "premium_amount": "400",
      "coverage_type": "Level",
      "sex": "Male",
      "state": "Nevada",
      "month": "12",
      "day": "11",
      "year": "1973",
      "feet": "5",
      "inches": "10",
      "pounds": "175",
      "nicotine_use": "None",
      "payment_type": "Bank Draft/EFT",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {},
    "drugs": {
      "Atorvastatin": {
        "indication": "High Cholesterol",
        "last_use_date": {
          "month": "Mar",
          "day": "10",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Apr",
          "day": "22",
          "year": "2023"
        }
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": "16000",
      "premium_amount": "500",
      "coverage_type": "Level",
      "sex": "Female",
      "state": "New York",
      "month": "1",
      "day": "25",
      "year": "1969",
      "feet": "5",
      "inches": "7",
      "pounds": "165",
      "nicotine_use": "None",
      "payment_type": "Credit Card",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {
      "Kidney Dialysis": {
        "Date of last treatment": {
          "month": "Feb",
          "day": "20",
          "year": "2024"
        },
        "Date of diagnosis?": {
          "month": "Mar",
          "day": "14",
          "year": "2019"
        },
        "checkbox_currently": "on"
      },
      "Oxygen continuous": {
        "Date of last treatment": {
          "month": "Apr",
          "day": "12",
          "year": "2023"
        },
        "currently_on": "off",
        "oxygen_use_for_cluster_headaches": "Yes",
        "chronic_respiratory_or_lung_problem": "Yes"
      }
    },
    "drugs": {
      "Methadone": {
        "indication": "Severe Pain",
        "last_use_date": {
          "month": "Apr",
          "day": "11",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "May",
          "day": "30",
          "year": "2023"
        },
        "carry_narcan": "Yes",
        "taking_medication_longer_6_months": "No"
      }
    }
  }
]
```

### Additional Documentation
All medications and health conditions will have their schemas explained in additional documentation to assist in the proper construction and submission of the JSON elements. Please refer to these documents for detailed schema information. 

### Postback Information
The client (Air.io) must inform the postback URL. For this initial phase, a temporary URL to view the postback is:  
[https://020524.bravog.com/itk_bot_postback.txt](https://020524.bravog.com/itk_bot_postback.txt)

### Modular System
The bot system is modular and can be extended to handle additional health conditions and medications/drugs. This allows for easy updates and integration of new requirements as they arise.

### Performance Note
Each quotation request takes an average of 20 to 30 seconds to be processed and posted back. The bot operates at a moderate speed due to limitations of the target host (insurancetoolkit.com). Some delays within this speed average are mandatory to keep the flows running flawlessly.
