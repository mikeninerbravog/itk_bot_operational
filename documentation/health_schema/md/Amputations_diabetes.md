### Amputations (related to diabetes): Constructing JSON Elements for ITK Bot

The JSON structure for Amputations (related to diabetes) includes the following fields:

- `Date of amputation`: The date the amputation occurred, broken down into `month`, `day`, and `year`.
- `wheelchair_confined`: Indicates whether the prospect is confined to a wheelchair (`"Yes"` or `"No"`).
- `a1c_reading_less_than_8`: Indicates whether the most recent A1C reading is less than 8 (`"Yes"` or `"No"`).
- `help_with_adls`: Indicates whether the prospect needs help with activities of daily living (ADLs) (`"Yes"` or `"No"`).

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
    "Amputations (related to diabetes)": {
      "Date of amputation": {
        "month": "Jun",
        "day": "12",
        "year": "2001"
      },
      "wheelchair_confined": "Yes",
      "a1c_reading_less_than_8": "No",
      "help_with_adls": "Yes"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
