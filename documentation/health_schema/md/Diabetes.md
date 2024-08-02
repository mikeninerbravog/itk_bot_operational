### Diabetes: Constructing JSON Elements for ITK Bot

The JSON structure for health conditions includes the following common fields for each condition:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis?`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.

Some conditions may include additional specific fields relevant to the condition.

#### Instructions

The JSON element for the condition must be nested under `"health_conditions":{}`.

#### Example Configurations

1. **Diabetes**

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
    "Diabetes": {
      "Date of last treatment": {
        "month": "Mar",
        "day": "11",
        "year": "2023"
      },
      "Date of diagnosis?": {
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
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

2. **Hypertension**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Hypertension": {
      "Date of last treatment": {
        "month": "Feb",
        "day": "20",
        "year": "2023"
      },
      "Date of diagnosis?": {
        "month": "Jan",
        "day": "15",
        "year": "2015"
      },
      "controlled_with_medication": "Yes",
      "taking_3_or_more_medications": "No",
      "recent_blood_pressure_reading": "120/80"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

3. **Asthma**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Asthma": {
      "Date of last treatment": {
        "month": "Apr",
        "day": "10",
        "year": "2024"
      },
      "Date of diagnosis?": {
        "month": "Jun",
        "day": "05",
        "year": "2010"
      },
      "hospitalizations_past_year": "No",
      "emergency_room_visits_past_year": "Yes",
      "uses_inhaler": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
