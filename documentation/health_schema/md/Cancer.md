### Cancer: Constructing JSON Elements for ITK Bot

The JSON structure for Cancer includes fields specific to various indications, such as Blood or Bone Marrow, Brain, Carcinoid or Neuroendocrine Tumor, and others. The fields are as follows:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis?`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `Had cancer more than once?`: Indicates whether the patient has had cancer more than once (`"Yes"` or `"No"`).
- `recurrent_cancer`: Indicates whether the cancer is recurrent (`"Yes"` or `"No"`).
- `metastatic_cancer`: Indicates whether the cancer is metastatic (`"Yes"` or `"No"`).
- `stage_beyond_1`: Indicates whether the cancer is beyond stage 1 (`"Yes"` or `"No"`).
- `stage_beyond_2`: Indicates whether the cancer is beyond stage 2 (`"Yes"` or `"No"`).
- `chemotherapy_past_12_months`: Indicates whether the patient has undergone chemotherapy in the past 12 months (`"Yes"` or `"No"`).

#### Instructions

The JSON element for the condition must be nested under `"health_conditions":{}`.

#### Example Configurations

1. **Blood or Bone Marrow**

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
    "Cancer": {
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

2. **Brain, Carcinoid or Neuroendocrine Tumor**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

3. **Hodgkin's Disease or Hodgkin's Lymphoma**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

4. **Leukemia**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

5. **Multiple Myeloma**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

6. **Non-Hodgkin's Lymphoma**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

7. **Pancreatic, Liver, or Ovarian**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

8. **Sarcoma, Lung, Head, or Neck**

```json
{
  "personal_info

": { ... },
  "health_conditions": {
    "Cancer": {
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

9. **Stage A Prostate**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

10. **Stomach, Esophageal, Small Intestine**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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

11. **Other**

```json
{
  "personal_info": { ... },
  "health_conditions": {
    "Cancer": {
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
