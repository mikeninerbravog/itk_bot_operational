### Lantus: Constructing JSON Elements for ITK Bot

The JSON structure for Lantus includes the following common fields for each indication:

- `indication`: The specific health condition for which Lantus is prescribed.
- `last_use_date`: The last date the medication was used, broken down into `month`, `day`, and `year`.
- `currently_taking_checkbox`: Indicates whether the patient is currently taking the medication (`"On"` or `"Off"`).
- `first_fill_date`: The first date the medication was prescribed, broken down into `month`, `day`, and `year`.
- `units_per_day`: The number of units of insulin taken per day.
- `uncontrolled_diabetes_past_10_years`: Indicates if diabetes has been uncontrolled in the past 10 years (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_past_3_years`: Indicates if diabetes has been uncontrolled in the past 3 years (`"Yes"` or `"No"`).
- `uncontrolled_diabetes_past_2_years`: Indicates if diabetes has been uncontrolled in the past 2 years (`"Yes"` or `"No"`).
- `recent_a1c_reading_less_than_8`: Indicates if the recent A1C reading is less than 8 (`"Yes"` or `"No"`).

#### Instructions

The JSON element for the drug must be nested under `"drugs":{}`.

#### Example Configurations

1. **Diabetes (No Complications)**

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
  // example of health_conditions: Please consult the documentation
  "health_conditions": {
    "Oxygen non continuous": {
      "Date of last treatment": {
        "month": "Apr",
        "day": "15",
        "year": "2010"
      },
      "checkbox_currently": "on",
      "daily_oxygen_use": "Yes",
      "oxygen_use_for_cluster_headaches": "No"
    }
  },
  "drugs": {
    "Lantus": {
      "indication": "Diabetes (No Complications)",
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
      "units_per_day": "5 units",
      "uncontrolled_diabetes_past_10_years": "Yes",
      "uncontrolled_diabetes_past_3_years": "Yes",
      "uncontrolled_diabetes_past_2_years": "Yes",
      "recent_a1c_reading_less_than_8": "No"
    }
  }
}
```

2. **Diabetic Nephropathy (Kidney)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Lantus": {
      "indication": "Diabetic Nephropathy (Kidney)",
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
      "units_per_day": "5 units",
      "uncontrolled_diabetes_past_2_years": "Yes",
      "recent_a1c_reading_less_than_8": "No"
    }
  }
}
```

3. **Diabetic Neuropathy (Nerve)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Lantus": {
      "indication": "Diabetic Neuropathy (Nerve)",
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
      "units_per_day": "5 units",
      "uncontrolled_diabetes_past_2_years": "Yes",
      "recent_a1c_reading_less_than_8": "No"
    }
  }
}
```
