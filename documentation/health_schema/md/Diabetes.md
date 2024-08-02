### Diabetes: Constructing JSON Elements for ITK Bot

The JSON structure for Diabetes includes the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `insulin_use`: Indicates whether the prospect uses insulin (`"Yes"` or `"No"`).
- `age_insulin_started`: The age at which the prospect started using insulin.
- `daily_insulin_units`: The number of insulin units taken daily.
- `uncontrolled_diabetes_past_10_years`: Indicates if diabetes has been uncontrolled in the past 10 years (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_past_3_years`: Indicates if diabetes has been uncontrolled in the past 3 years (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_past_2_years`: Indicates if diabetes has been uncontrolled in the past 2 years (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_past_year`: Indicates if diabetes has been uncontrolled in the past year (`"Yes"` or `"No"`).
- `changes_in_medications_past_year`: Indicates if there have been changes in diabetes medications in the past year (`"Yes"` or `"No"`).
- `taking_3_or_more_medications`: Indicates if the prospect is taking three or more medications for diabetes (`"Yes"` or `"No"`).
- `a1c_reading_less_than_8`: Indicates if the A1C reading is less than 8 (`"Yes"` or `"No"`).
- `a1c_reading_between_8_8_6`: Indicates if the A1C reading is between 8 and 8.6 (`"Yes"` or `"No"`).
- `a1c_reading_between_8_7_9_9`: Indicates if the A1C reading is between 8.7 and 9.9 (`"Yes"` or `"No"`).
- `a1c_reading_between_10_11`: Indicates if the A1C reading is between 10 and 11 (`"Yes"` or `"No"`).

#### Instructions

The JSON element for the condition must be nested under `"health_conditions":{}`.

#### Example Configuration

```json
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
    "Diabetes": {
      "Date of last treatment": {
        "month": "Mar",
        "day": "11",
        "year": "2023"
      },
      "Date of diagnosis": {
        "month": "Nov",
        "day": "12",
        "year": "2018"
      },
      "insulin_use": "No",
      "age_insulin_started": "12",
      "daily_insulin_units": "20 units",
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
    }
  },
  "drugs": {
    "Valium": { ... }
  }
}
```
