### Metoprolol: Constructing JSON Elements for ITK Bot

The JSON structure for Metoprolol includes the following common fields for each indication:

- `indication`: The specific health condition for which Metoprolol is prescribed.
- `last_use_date`: The last date the medication was used, broken down into `month`, `day`, and `year`.
- `currently_taking_checkbox`: Indicates whether the patient is currently taking the medication (`"On"` or `"Off"`).
- `first_fill_date`: The first date the medication was prescribed, broken down into `month`, `day`, and `year`.

Some conditions may include additional specific fields relevant to the indication.

#### Instructions

The JSON element for the drug must be nested under `"drugs":{}`.

#### Example Configurations

1. **Angina (Chest Pain)**

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
    "Metoprolol": {
      "indication": "Angina (Chest Pain)",
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
      }
    }
  }
}
```

2. **Atrial Fibrillation (AFIB)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "Atrial Fibrillation (AFIB)",
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
      "episode_afib_last_12_months": "No"
    }
  }
}
```

3. **CHF (Congestive Heart Failure)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "CHF (Congestive Heart Failure)",
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
      }
    }
  }
}
```

4. **Heart Attack**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "Heart Attack",
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
      "more_than_1_heart_attack": "No"
    }
  }
}
```

5. **High Blood Pressure (Controlled)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "High Blood Pressure (Controlled)",
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
      "compliant_taking_medication": "Yes"
    }
  }
}
```

6. **High Blood Pressure (Uncontrolled)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "High Blood Pressure (Uncontrolled)",
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
      "high_bp_reading": "No"
    }
  }
}
```

7. **Thrombosis (Blood Clots)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Metoprolol": {
      "indication": "Thrombosis (Blood Clots)",
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
      "chronic_pulmonary_embolism": "No"
    }
  }
}
```
