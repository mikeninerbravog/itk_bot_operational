### Stroke: Constructing JSON Elements for ITK Bot

The JSON structure for Stroke includes the following fields:

- `Date of occurrence`: The date the stroke occurred, broken down into `month`, `day`, and `year`.
- `had_more_than_one_stroke`: Indicates whether the individual had more than one stroke (`"Yes"` or `"No"`).
- `had_two_or_more_strokes_past_3_years`: Indicates whether the individual had two or more strokes in the past three years (`"Yes"` or `"No"`).

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
    "Stroke": {
      "Date of occurrence": {
        "month": "Mar",
        "day": "11",
        "year": "2023"
      },
      "had_more_than_one_stroke": "Yes",
      "had_two_or_more_strokes_past_3_years": "No"
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
    "Stroke": {
      "Date of occurrence": {
        "month": "Mar",
        "day": "11",
        "year": "2023"
      },
      "had_more_than_one_stroke": "Yes",
      "had_two_or_more_strokes_past_3_years": "No"
    }
  },
  "drugs": {
    // Please, consult the documentation of the drug/medication
    "Valium": { ... }
  }
}
```
