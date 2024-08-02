# Example #2 Session with 4 Quotation Requests

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
      "coverage_amount": "12000",
      "premium_amount": null,
      "coverage_type": "Level",
      "sex": "Male",
      "state": "Colorado",
      "month": "5",
      "day": "21",
      "year": "1974",
      "feet": "5",
      "inches": "8",
      "pounds": "160",
      "nicotine_use": "None",
      "payment_type": "Credit Card",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {
      "Schizophrenia": {
        "Date of last treatment": {
          "month": "Mar",
          "day": "11",
          "year": "2023"
        },
        "Date of diagnosis": {
          "month": "Jun",
          "day": "9",
          "year": "2008"
        },
        "requiring_inpatient_treatment_past_2_years": "Yes"
      },
      "Kidney Stones": {
        "Date of last treatment": {
          "month": "Jul",
          "day": "19",
          "year": "2023"
        }
      }
    },
    "drugs": {
      "Aspirin": {
        "indication": "Angina (Chest Pain)",
        "last_use_date": {
          "month": "Mar",
          "day": "11",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Jun",
          "day": "30",
          "year": "2023"
        }
      },
      "Lipitor": {
        "indication": "High Cholesterol",
        "last_use_date": {
          "month": "Jul",
          "day": "21",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Sep",
          "day": "10",
          "year": "2023"
        }
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": null,
      "premium_amount": "55",
      "coverage_type": "Level",
      "sex": "Female",
      "state": "Illinois",
      "month": "11",
      "day": "18",
      "year": "1963",
      "feet": "5",
      "inches": "6",
      "pounds": "155",
      "nicotine_use": "None",
      "payment_type": "Bank Draft/EFT",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {
      "Alzheimer's disease": {
        "date_last_treatment": {
          "month": "Jun",
          "day": "18",
          "year": "2023"
        },
        "date_of_diagnosis": {
          "month": "Jan",
          "day": "6",
          "year": "2021"
        },
        "prospect_has_alzheimers": "No",
        "prospect_has_dementia": "Yes"
      }
    },
    "drugs": {
      "Carvedilol": {
        "indication": "High Blood Pressure (Controlled)",
        "last_use_date": {
          "month": "Feb",
          "day": "15",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Mar",
          "day": "12",
          "year": "2023"
        },
        "compliant_medication": "Yes"
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": "9000",
      "premium_amount": null,
      "coverage_type": "Level",
      "sex": "Male",
      "state": "Georgia",
      "month": "7",
      "day": "30",
      "year": "1977",
      "feet": "6",
      "inches": "0",
      "pounds": "175",
      "nicotine_use": "Cigarettes",
      "payment_type": "Credit Card",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {
      "Cancer": {
        "Indication": {
          "Multiple Myeloma": {
            "Date of last treatment": {
              "month": "Jun",
              "day": "12",
              "year": "2001"
            },
            "Date of diagnosis?": {
              "month": "Mar",
              "day": "28",
              "year": "2005"
            },
            "Had cancer more than once?": "Yes",
            "recurrent_cancer": "No",
            "metastatic_cancer": "Yes",
            "stage_beyond_1": "Yes",
            "stage_beyond_2": "No",
            "chemotherapy_past_12_months": "No"
          }
        }
      },
      "Diabetes": {
        "Date of last treatment": {
          "month": "Apr",
          "day": "9",
          "year": "2023"
        },
        "Date of diagnosis?": {
          "month": "May",
          "day": "17",
          "year": "2020"
        },
        "insulin_use": "No",
        "age_insulin_started": "15",
        "daily_insulin_units": "30 units",
        "uncontrolled_diabetes_past_10_years": "No",
        "uncontrolled_diabetes_past_3_years": "No",
        "uncontrolled_diabetes_past_2_years": "No",
        "uncontrolled_diabetes_past_year": "Yes",
        "changes_in_medications_past_year": "Yes",
        "taking_3_or_more_medications": "Yes",
        "a1c_reading_less_than_8": "Yes",
        "a1c_reading_between_8_8_6": "No",
        "a1c_reading_between_8_7_9_9": "No",
        "a1c_reading_between_10_11": "No"
      }
    },
    "drugs": {
      "Metformin": {
        "indication": "Diabetes (No Complications)",
        "last_use_date": {
          "month": "May",
          "day": "11",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Jul",
          "day": "19",
          "year": "2023"
        },
        "uncontrolled_diabetes_past_10_years": "Yes",
        "uncontrolled_diabetes_past_3_years": "Yes",
        "uncontrolled_diabetes_past_2_years": "Yes",
        "uncontrolled_diabetes_past_year": "Yes",
        "medication_changes": "No",
        "a1c_reading_less_than_8": "No",
        "a1c_reading_between_8_and_8_6": "Yes"
      }
    }
  },
  {
    "personal_info": {
      "coverage_amount": "6000",
      "premium_amount": null,
      "coverage_type": "Level",
      "sex": "Female",
      "state": "Arizona",
      "month": "3",
      "day": "12",
      "year": "1969",
      "feet": "5",
      "inches": "5",
      "pounds": "150",
      "nicotine_use": "None",
      "payment_type": "Bank Draft/EFT",
      "callSID": "CAabcdef123456abcdef1234567890abcd",
      "phone": "(602) 123-4567"
    },
    "health_conditions": {},
    "drugs": {
      "Eliquis": {
        "indication": "Thrombosis (Blood Clots)",
        "last_use_date": {
          "month": "Jun",
          "day": "19",

          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Aug",
          "day": "8",
          "year": "2023"
        },
        "multiple_blood_clots": "Yes",
        "chronic_pulmonary_embolism": "Yes"
      },
      "Lisinopril": {
        "indication": "High Blood Pressure (Controlled)",
        "last_use_date": {
          "month": "Jan",
          "day": "22",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Mar",
          "day": "12",
          "year": "2023"
        },
        "compliant_with_medication": "Yes"
      }
    }
  }
]
```

## Additional Information

The client must inform additional `key:value` pairs to match their project requirements. These will be deployed in the automated system accordingly.
