### Metformin: Constructing JSON Elements for ITK Bot

The JSON structure for Metformin includes the following common fields for each indication:

- `indication`: The specific health condition for which Metformin is prescribed.
- `last_use_date`: The last date the medication was used, broken down into `month`, `day`, and `year`.
- `currently_taking_checkbox`: Indicates whether the patient is currently taking the medication (`"On"` or `"Off"`).
- `first_fill_date`: The first date the medication was prescribed, broken down into `month`, `day`, and `year`.

Some conditions may include additional specific fields relevant to the indication.

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
    "Metformin": {
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
      "uncontrolled_diabetes_past_10_years": "Yes",
      "uncontrolled_diabetes_past_3_years": "Yes",
      "uncontrolled_diabetes_past_2_years": "Yes",
      "uncontrolled_diabetes_past_year": "Yes",
      "medication_changes": "No",
      "a1c_reading_less_than_8": "No",
      "a1c_reading_between_8_and_8_6": "Yes"
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
    "Metformin": {
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
      "uncontrolled_diabetes_past_2_years": "Yes",
      "a1c_reading_less_than_8": "No",
      "a1c_reading_between_8_and_8_6": "Yes"
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
    "Metformin": {
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
      "uncontrolled_diabetes_past_2_years": "Yes",
      "a1c_reading_less_than_8": "No",
      "a1c_reading_between_8_and_8_6": "Yes"
    }
  }
}
```
