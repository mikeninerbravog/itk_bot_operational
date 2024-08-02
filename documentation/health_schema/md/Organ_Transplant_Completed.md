### Organ Transplant (Completed): Constructing JSON Elements for ITK Bot

The JSON structure for Organ Transplant (Completed) includes the following fields:

- `Date of occurrence`: The date the transplant occurred, broken down into `month`, `day`, and `year`.
- `stage_cirrhosis`: Indicates whether the patient has cirrhosis (`"Yes"` or `"No"`).

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
    "Organ Transplant (Completed)": {
      "Indication": {
        "Heart Transplant": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

```json
{
  // personal_info: Please populate with your own data
  "personal_info": { ... },
  "health_conditions": {
    "Organ Transplant (Completed)": {
      "Indication": {
        "Kidney Transplant": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

```json
{
  // personal_info: Please populate with your own data
  "personal_info": { ... },
  "health_conditions": {
    "Organ Transplant (Completed)": {
      "Indication": {
        "Liver Transplant": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

```json
{
  // personal_info: Please populate with your own data
  "personal_info": { ... },
  "health_conditions": {
    "Organ Transplant (Completed)": {
      "Indication": {
        "Lung Transplant": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

```json
{
  // personal_info: Please populate with your own data
  "personal_info": { ... },
  "health_conditions": {
    "Organ Transplant (Completed)": {
      "Indication": {
        "Pancreas Transplant": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```

```json
{
  // personal_info: Please populate with your own data
  "personal_info": { ... },
  "health_conditions": {
    "Organ Transplant (Completed)": {
      "Indication": {
        "Other": {
          "Date of occurrence": {
            "month": "Mar",
            "day": "11",
            "year": "2023"
          },
          "stage_cirrhosis": "Yes"
        }
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
