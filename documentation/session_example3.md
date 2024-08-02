# Example #3 Session with 5 Quotation Requests

## Submission URL

To post the JSON element, use the following URL:  
[https://itkbot.bravog.com/upload-config](https://itkbot.bravog.com/upload-config)

## Real-Time Log Access

To access the real-time log of the current session operation, visit:  
[https://itkbot.bravog.com/view-logs](https://itkbot.bravog.com/view-logs)

## Temporary Postback URL

For viewing results, the temporary postback URL is:  
[https://020524.bravog.com/itk_bot_postback.txt](https://020524.bravog.com/itk_bot_postback.txt)  
**Note**: The client must provide their postback URL.

## Resetting the Postback Log

To reset (empty) the postback log content, access or trigger:  
[https://020524.bravog.com/itk-postback-reseting/](https://020524.bravog.com/itk-postback-reseting/)

## Example of 5 Quotation Requests

```json
[
  {
    "personal_info": {
      "coverage_amount": null,
      "premium_amount": "350",
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
      "phone": "(602) 123-4567"
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

## Additional Information

The client must inform additional `key:value` pairs to match their project requirements. These will be deployed in the automated system accordingly.
