### Plavix: Constructing JSON Elements for ITK Bot

The JSON structure for Plavix includes the following common fields for each indication:

- `indication`: The specific health condition for which Plavix is prescribed.
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
    "Plavix": {
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
      },
      "dosage_over_75mg": "Yes"
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
    "Plavix": {
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
      "dosage_over_75mg": "Yes",
      "episode_afib_last_12_months": "Yes"
    }
  }
}
```

3. **Heart Attack**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Plavix": {
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
      "dosage_over_75mg": "Yes",
      "more_than_1_heart_attack": "Yes"
    }
  }
}
```

4. **Heart Surgery**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Plavix": {
      "indication": "Heart Surgery",
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
      "dosage_over_75mg": "Yes",
      "surgery_to_implant_defibrillator": "Yes"
    }
  }
}
```

5. **Peripheral Artery Disease (PAD)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Plavix": {
      "indication": "Peripheral Artery Disease (PAD)",
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
      "dosage_over_75mg": "Yes"
    }
  }
}
```

6. **Stroke**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Plavix": {
      "indication": "Stroke",
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
      "dosage_over_75mg": "Yes",
      "more_than_1_stroke": "Yes"
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
    "Plavix": {
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
      "dosage_over_75mg": "Yes",
      "chronic_pulmonary_embolism": "Yes"
    }
  }
}
```

8. **Transient Ischemic Attack (TIA or Mini-Stroke)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Plavix": {
      "indication": "Transient Ischemic Attack (TIA or Mini-Stroke)",
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
      "more_than_1_tia": "Yes",
      "more_than_1_stroke": "Yes",
      "two_or_more_strokes_past_3_years": "Yes"
    }
  }
}
```
