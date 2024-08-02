# ITK Bot

- **Codename: ITK Bot Mike Beta 1**
- **Version 1 (Jun 2024)**
- **Developed by Mike Niner Bravog aka Marcello Dev @ Upwork**  
- **Client: Air.io**

### Submission URL

To post the JSON element, use the following URL:  
[https://itkbot.bravog.com/upload-config](https://itkbot.bravog.com/upload-config)

### Postback Information

The client (Air.io) must inform the postback URL. For this initial phase, a temporary URL to view the postback is:  
[https://020524.bravog.com/itk_bot_postback.txt](https://020524.bravog.com/itk_bot_postback.txt)

### Example JSON Element

```json
[
  {
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
      "Alcohol abuse": {
        "Date of last treatment": {
          "month": "Jun",
          "day": "18",
          "year": "2023"
        },
        "narcotics_abuse": "Yes"
      },
      "Diabetes": {
        "Date of last treatment": {
          "month": "Mar",
          "day": "14",
          "year": "2023"
        },
        "Date of diagnosis?": {
          "month": "Nov",
          "day": "22",
          "year": "2019"
        },
        "insulin_use": "No",
        "age_insulin_started": "14",
        "daily_insulin_units": "25 units",
        "uncontrolled_diabetes_past_10_years": "No",
        "uncontrolled_diabetes_past_3_years": "No",
        "uncontrolled_diabetes_past_2_years": "No",
        "uncontrolled_diabetes_past_year": "Yes",
        "changes_in_medications_past_year": "No",
        "taking_3_or_more_medications": "Yes",
        "a1c_reading_less_than_8": "Yes",
        "a1c_reading_between_8_8_6": "No",
        "a1c_reading_between_8_7_9_9": "No",
        "a1c_reading_between_10_11": "No"
      },
      "Heart attack": {
        "Date of occurrence": {
          "month": "Aug",
          "day": "5",
          "year": "2022"
        },
        "multiple_heart_attacks": "Yes"
      }
    },
    "drugs": {
      "Plavix": {
        "indication": "Atrial Fibrillation (AFIB)",
        "last_use_date": {
          "month": "May",
          "day": "7",
          "year": "2024"
        },
        "currently_taking_checkbox": "On",
        "first_fill_date": {
          "month": "Jul",
          "day": "19",
          "year": "2023"
        },
        "dosage_over_75mg": "Yes",
        "episode_afib_last_12_months": "Yes"
      }
    }
  }
]
```

## Overview

ITK Bot is a powerful tool designed to automate the process of filling out insurance quotation forms on insurancetoolkit.com, specifically within the "FEX" section. This bot aims to help insurance agents perform their jobs more efficiently by handling a high volume of quotes daily and responding to dynamic form questions.

## Features

- **Automated Form Filling:** The bot can log in and automatically fill out insurance quotation forms quickly and accurately.
- **High Volume Processing:** Capable of handling hundreds even thousands of quotes per day without breaking.
- **High Speed:** Each Final Expense Quote takes from 20 to 30 seconds on average to get done.
- **Dynamic Question Handling:** Smart to answer additional questions that appear based on the information entered.
- **Integration with Existing Systems:** Designed to work seamlessly with current systems at insurancetoolkit.com.

### Instructions of JSON Element Constructing
Including URL Endpoint and post-back instructions
- [General explanation about the JSON Element that trigger the ITK Bot](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/ITK_Bot_release.md)


### Health Conditions JSON Schemas:

- [AIDS HIV ARC](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/AIDS_HIV_ARC.md)
- [Alcohol abuse](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Alcohol_abuse.md)
- [Alzheimers Disease](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Alzheimers_Disease.md)
- [Amputations diabetes](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Amputations_diabetes.md)
- [Cancer](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Cancer.md)
- [COPD](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/COPD.md)
- [COVID-19](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/COVID-19.md)
- [Dementia](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Dementia.md)
- [Diabetes](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Diabetes.md)
- [Diabetic coma](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Diabetic_coma.md)
- [Diabetic neuropathy](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Diabetic_neuropathy.md)
- [Diabetic retinopathy](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Diabetic_retinopathy.md)
- [Heart Attack](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Heart_Attack.md)
- [Hepatitis A Chronic](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_A_Chronic.md)
- [Hepatitis A Cured](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_A_Cured.md)
- [Hepatitis B Chronic](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_B_Chronic.md)
- [Hepatitis B Cured](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_B_Cured.md)
- [Hepatitis C Chronic](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_C_Chronic.md)
- [Hepatitis C Cured](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Hepatitis_C_Cured.md)
- [High Blood Pressure](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/High_Blood_Pressure.md)
- [High Cholesterol](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/High_Cholesterol.md)
- [Kidney Dialysis](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Kidney_Dialysis.md)
- [Kidney Stones](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Kidney_Stones.md)
- [Memory Loss](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Memory_Loss.md)
- [Organ Transplant Completed](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Organ_Transplant_Completed.md)
- [Oxygen Continuous](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Oxygen_Continuous.md)
- [Oxygen Non Continuous](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Oxygen_Non_Continuous.md)
- [Past cancer](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Past_cancer.md)
- [Schizophrenia](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Schizophrenia.md)
- [Stroke](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/health_schema/md/Stroke.md)

### Medications JSON Schemas:

- [Amlodipine](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Amlodipine.md)
- [Aspirin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Aspirin.md)
- [Atenolol](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Atenolol.md)
- [Atorvastatin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Atorvastatin.md)
- [Carvedilol](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Carvedilol.md)
- [Celebrex](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Celebrex.md)
- [Diltiazem](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Diltiazem.md)
- [Eliquis](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Eliquis.md)
- [Entresto](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Entresto.md)
- [Ezetimibe](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Ezetimibe.md)
- [Gabapentin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Gabapentin.md)
- [Insulin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Insulin.md)
- [Lantus](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lantus.md)
- [Lasix](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lasix.md)
- [Lipitor](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lipitor.md)
- [Lisinopril](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lisinopril.md)
- [Lithium](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lithium.md)
- [Losartan](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Losartan.md)
- [Lovastatin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lovastatin.md)
- [Lyrica](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Lyrica.md)
- [Meloxicam](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Meloxicam.md)
- [Metformin](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Metformin.md)
- [Methadone](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Methadone.md)
- [Metoprolol](https://github.com/mikeninerbravog/itk_bot_operational/blob/master/documentation/medications_schema/md/Metoprolol.md)
