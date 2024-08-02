### Diabetic Retinopathy: Constructing JSON Elements for ITK Bot

The JSON structure for Diabetic Retinopathy includes the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `insulin_use`: Indicates whether the prospect uses insulin (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_2_years`: Indicates if diabetes has been uncontrolled in the past 2 years (`"Yes"` or `"No"`).
- `a1c_reading_less_than_8`: Indicates if the A1C reading is less than 8 (`"Yes"` or `"No"`).
- `a1c_reading_between_8_8_6`: Indicates if the A1C reading is between 8 and 8.6 (`"Yes"` or `"No"`).
- `a1c_reading_between_8_7_9_9`: Indicates if the A1C reading is between 8.7 and 9.9 (`"Yes"` or `"No"`).
- `a1c_reading_between_10_11`: Indicates if the A1C reading is between 10 and 11 (`"Yes"` or `"No"`).

#### Instructions

The JSON element for the condition must be nested under `"health_conditions":{}`.

#### Example Configuration

```json
{
  // personal_info: Please populate with your own data
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
    "Diabetic retinopathy": {
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
      "insulin_use": "Yes",
      "uncontrolled_diabetes_2_years": "No",
      "a1c_reading_less_than_8": "Yes",
      "a1c_reading_between_8_8_6": "Yes",
      "a1c_reading_between_8_7_9_9": "Yes",
      "a1c_reading_between_10_11": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
