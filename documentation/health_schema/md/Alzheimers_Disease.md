### Alzheimer's Disease: Constructing JSON Elements for ITK Bot

The JSON structure for Alzheimer's Disease includes the following fields:

- `date_last_treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `date_of_diagnosis`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `prospect_has_alzheimers`: Indicates whether the prospect has Alzheimer's disease (`"Yes"` or `"No"`).
- `prospect_has_dementia`: Indicates whether the prospect has dementia (`"Yes"` or `"No"`).

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
    "Alzheimer's disease": {
      "date_last_treatment": {
        "month": "Jun",
        "day": "18",
        "year": "2023"
      },
      "date_of_diagnosis": {
        "month": "Jan",
        "day": "6",
        "year": "2021"
      },
      "prospect_has_alzheimers": "No",
      "prospect_has_dementia": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
