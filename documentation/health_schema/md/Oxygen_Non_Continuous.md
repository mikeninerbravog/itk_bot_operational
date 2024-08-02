### Oxygen Non Continuous: Constructing JSON Elements for ITK Bot

The JSON structure for Oxygen Non Continuous includes the following fields:

- `Date of last treatment`: The last date the condition was treated, broken down into `month`, `day`, and `year`.
- `checkbox_currently`: Indicates whether the patient is currently using non-continuous oxygen (`"on"` or `"off"`).
- `daily_oxygen_use`: Indicates if the oxygen is used daily (`"Yes"` or `"No"`).
- `oxygen_use_for_cluster_headaches`: Indicates if the oxygen is used for cluster headaches (`"Yes"` or `"No"`).

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
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
