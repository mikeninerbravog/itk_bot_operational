### Eliquis: Constructing JSON Elements for ITK Bot

The JSON structure for Eliquis includes the following common fields for each indication:

- `indication`: The specific health condition for which Eliquis is prescribed.
- `last_use_date`: The last date the medication was used, broken down into `month`, `day`, and `year`.
- `currently_taking_checkbox`: Indicates whether the patient is currently taking the medication (`"On"` or `"Off"`).
- `first_fill_date`: The first date the medication was prescribed, broken down into `month`, `day`, and `year`.

Some conditions may include additional specific fields relevant to the indication.

#### Instructions

The JSON element for the drug must be nested under `"drugs":{}`.

#### Example Configurations

1. **Atrial Fibrillation (AFIB)**

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
    "Eliquis": {
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
      "afib_episode_last_12_months": "Yes"
    }
  }
}
```

2. **Circulatory Disease**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
      "indication": "Circulatory Disease",
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

3. **Circulatory Surgery (Heart or brain)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
      "indication": "Circulatory Surgery (Heart or brain)",
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

4. **Circulatory Surgery (Other)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
      "indication": "Circulatory Surgery (Other)",
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

5. **Heart Arrhythmia**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
      "indication": "Heart Arrhythmia",
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
      "afib_episode_last_12_months": "Yes"
    }
  }
}
```

6. **Heart Surgery (Defibrillator Implant)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
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
      "defibrillator_implant": "Yes"
    }
  }
}
```

7. **Heart Surgery (Multiple Blood Clots)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
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
      "multiple_blood_clots": "Yes"
    }
  }
}
```

8. **Thrombosis (Blood Clots)**

```json
{
  "personal_info": { ... },
  "health_conditions": { ... },
  "drugs": {
    "Eliquis": {
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
      "multiple_blood_clots": "Yes",
      "chronic_pulmonary_embolism": "Yes"
    }
  }
}
```
