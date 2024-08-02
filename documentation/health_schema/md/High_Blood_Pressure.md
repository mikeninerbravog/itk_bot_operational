### High Blood Pressure: Constructing JSON Elements for ITK Bot

The JSON structure for High Blood Pressure includes the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `Date of diagnosis?`: The date the condition was diagnosed, broken down into `month`, `day`, and `year`.
- `medication_compliance`: Indicates whether the prospect is compliant with medication (`"Yes"` or `"No"`).

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
    "High blood pressure": {
      "Date of last treatment": {
        "month": "Jan",
        "day": "1",
        "year": "2023"
      },
      "Date of diagnosis?": {
        "month": "Jan",
        "day": "1",
        "year": "2023"
      },
      "medication_compliance": "No"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
