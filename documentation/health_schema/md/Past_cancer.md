### Past Cancer: Constructing JSON Elements for ITK Bot

The JSON structure for Past Cancer includes various indications with specific fields. Each indication has the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis?`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `Had cancer more than once?`: Indicates if the patient had cancer more than once (`"Yes"` or `"No"`).
- `recurrent_cancer`: Indicates if the cancer is recurrent (`"Yes"` or `"No"`).
- `metastatic_cancer`: Indicates if the cancer is metastatic (`"Yes"` or `"No"`).
- `stage_beyond_1`: Indicates if the cancer is beyond stage 1 (`"Yes"` or `"No"`).
- `stage_beyond_2`: Indicates if the cancer is beyond stage 2 (`"Yes"` or `"No"`).
- `chemotherapy_past_12_months`: Indicates if the patient underwent chemotherapy in the past 12 months (`"Yes"` or `"No"`).

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
    "Past cancer": {
      "Indication": {
        "Blood or Bone Marrow": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Brain, Carcinoid or Neuroendocrine Tumor": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Hodgkin's Disease or Hodgkin's Lymphoma": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Leukemia": {
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
  "health_conditions": {
    "Past cancer": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Non-Hodgkin's Lymphoma": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Pancreatic, Liver, or Ovarian": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Sarcoma, Lung, Head, or Neck": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Stage A Prostate": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Stomach, Esophageal, Small Intestine": {
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
  "health_conditions": {
    "Past cancer": {
      "Indication": {
        "Other": {
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
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
