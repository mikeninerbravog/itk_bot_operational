### Heart Attack: Constructing JSON Elements for ITK Bot

The JSON structure for Heart Attack includes the following fields:

- `Date of occurrence`: The date the heart attack occurred, broken down into `month`, `day`, and `year`.
- `multiple_heart_attacks`: Indicates whether the prospect has had multiple heart attacks (`"Yes"` or `"No"`).

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
    "Heart attack": {
      "Date of occurrence": {
        "month": "Mar",
        "day": "11",
        "year": "2023"
      },
      "multiple_heart_attacks": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
