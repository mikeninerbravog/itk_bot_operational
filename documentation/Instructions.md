# JSON Element Explanation

## Personal Information

### Example JSON Element
```json
{
  "personal_info": {
    "coverage_amount": "19000",
    "premium_amount": "70",
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
    "callSID": "CAabcdef123456abcdef1234567890abcd",  // YOU must inform this
    "phone": "(602) 123-4567"  // You must inform this
  }
}
```

### Detailed Explanation

#### Coverage and Premium Amounts
- If both `coverage_amount` and `premium_amount` are provided:
  ```json
  "coverage_amount": "19000",
  "premium_amount": "70"
  ```
  Only `premium_amount` will be considered.

- If only `premium_amount` is provided:
  ```json
  "coverage_amount": null,
  "premium_amount": "70"
  ```
  `premium_amount` will be considered.

- If only `coverage_amount` is provided:
  ```json
  "coverage_amount": "19000",
  "premium_amount": null
  ```
  `coverage_amount` will be considered.

#### Coverage Type
The type of insurance coverage can be one of the following (as strings):
- `"Level"`
- `"Graded/Modified"`
- `"Guaranteed"`
- `"Limited Pay"`

#### Sex
The sex of the individual can be one of the following (as strings):
- `"Male"`
- `"Female"`

#### State
The state of residence can be any of the 51 US states (as strings).

#### Birthday
The birthdate of the individual, broken down into:
- `"month"`: A number from `"1"` to `"12"` representing the month of birth.
- `"day"`: A number from `"1"` to `"31"` representing the day of birth.
- `"year"`: A four-digit year representing the year of birth, e.g., `"1980"`.

#### Height/Weight
The height and weight of the individual, represented by:
- `"feet"`: The number of feet in height, e.g., `"5"`.
- `"inches"`: The number of inches in height, e.g., `"6"`.
- `"pounds"`: The weight in pounds, e.g., `"140"`.

#### Nicotine Use
The nicotine use status of the individual, which can be one of the following (as strings):
- `"None"`
- `"Cigarettes"`
- `"Cigarettes + Other Nicotine Products"`
- `"Occasional pipe/cigar use only"`
- `"Other Nicotine Products"`

#### Payment Type
The preferred payment method, which can be one of the following (as strings):
- `"Bank Draft/EFT"`
- `"Direct Express"`
- `"Credit Card"`
- `"Debit Card"`

### Note
All values must be strings (str) embraced with double quotes `"..."`.

### Required Fields
- `"callSID": "CAabcdef123456abcdef1234567890abcd"`: You must inform this.
- `"phone": "(602) 123-4567"`: You must inform this.
