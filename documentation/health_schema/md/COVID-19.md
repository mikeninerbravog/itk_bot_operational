### COVID-19: Constructing JSON Elements for ITK Bot

The JSON structure for COVID-19 includes the following fields:

- `Date cured`: The date the condition was cured, broken down into `month`, `day`, and `year`.
- `hospitalized_past_6_months`: Indicates whether the prospect was hospitalized in the past 6 months (`"Yes"` or `"No"`).
- `hospitalized_past_year`: Indicates whether the prospect was hospitalized in the past year (`"Yes"` or `"No"`).
- `icu_past_2_years`: Indicates whether the prospect was in the ICU in the past 2 years (`"Yes"` or `"No"`).

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
    "COVID-19": {
      "Date cured": {
        "month": "May",
        "day": "10",
        "year": "2022"
      },
      "hospitalized_past_6_months": "No",
      "hospitalized_past_year": "Yes",
      "icu_past_2_years": "No"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
