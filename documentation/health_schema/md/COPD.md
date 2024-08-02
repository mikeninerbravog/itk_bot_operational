### COPD: Constructing JSON Elements for ITK Bot

The JSON structure for COPD includes the following fields:

- `last_treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `diagnosis`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `nebulizer_use`: Indicates whether the prospect uses a nebulizer (`"Yes"` or `"No"`).
- `three_or_more_medications`: Indicates whether the prospect is taking three or more medications for the condition (`"Yes"` or `"No"`).

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
    "COPD": {
      "last_treatment": {
        "month": "Apr",
        "day": "12",
        "year": "2001"
      },
      "diagnosis": {
        "month": "Nov",
        "day": "18",
        "year": "1999"
      },
      "nebulizer_use": "Yes",
      "three_or_more_medications": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
