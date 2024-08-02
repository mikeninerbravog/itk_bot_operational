### High Cholesterol: Constructing JSON Elements for ITK Bot

The JSON structure for High Cholesterol includes the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.

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
    "High cholesterol": {
      "Date of last treatment": {
        "month": "Jan",
        "day": "1",
        "year": "2023"
      }
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
