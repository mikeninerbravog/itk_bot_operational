### ITK Bot - Documentation

- **Codename: ITK Bot Mike Beta 1**
- **Version 1 (Jun 2024)**
- **Developed by Mike Niner Bravog**  

### Submission URL

To post the JSON element, use the following URL:  
[https://itkbot.bravog.com/upload-config](https://itkbot.bravog.com/upload-config)

### Postback Information (temporary)

The client (Air.ai) must inform the postback URL. For this initial phase, a temporary URL to view the postback is:  
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
**Update: You can test for free for 14 days. After that keep using it for a small monthly fee.**

ITK Bot is a powerful tool designed to automate the process of filling out insurance quotation forms on insurancetoolkit.com, specifically within the "FEX" section. This bot aims to help insurance agents perform their jobs more efficiently by handling a high volume of quotes daily and responding to dynamic form questions.

## Features

- **Automated Form Filling:** The bot can log in and automatically fill out insurance quotation forms quickly and accurately.
- **High Volume Processing:** Capable of handling hundreds even thousands of quotes per day without breaking.
- **High Speed:** Each Final Expense Quote takes from 20 to 30 seconds on average to get done.
- **Dynamic Question Handling:** Smart to answer additional questions that appear based on the information entered.
- **Integration with Existing Systems:** Designed to work seamlessly with current systems at insurancetoolkit.com.
- **Queue Processing:** The system supports the processing of multiple JSON elements posted continuously in the same session. The bot processes all items in the queue sequentially, in the order they are received. This feature ensures that the system can handle a high volume of requests efficiently and without interruption.

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

### General Notes

This bot system was programmed to get the job done flawlessly, but as it depends on host resources and structure, some issues may occur. Despite thorough programming and testing, external factors such as server limitations, UI changes, and unexpected pop-up questions from the host can impact the bot's performance. Understanding these dependencies is crucial for maintaining and updating the system effectively.

1. **Insurance Toolkit Server Limitations**:
   - The bot's processing speed is constrained by the response times and limitations of the Insurance Toolkit servers. Each quotation request takes an average of 20 to 30 seconds to process due to these limitations.

2. **Valid Insurance Toolkit Account**:
   - A valid and active Insurance Toolkit account (login/password) is required for the ITK Bot to function correctly. Without proper credentials, the bot will not be able to access the necessary tools and perform its tasks as expected.

3. **Single Connection Per IP**:
   - The Insurance Toolkit server only permits one connection per IP address at a time. If more than one connection occurs simultaneously from the same IP, the host system terminates both the original and the additional connections. This limitation must be carefully managed to avoid disruptions.

4. **Handling Pop-up Questions**:
   - The bot needs to be capable of handling additional questions that may pop up during the form submission process. These pop-ups or in-line suggestions are often generated by the host and sometimes cannot be triggered by the bot. In some cases, unexpected questions or new fields may cause the bot to fail if not properly accounted for in the initial setup. In such cases, the quote may not be completed for that request, but the bot will make an attempt to handle these situations and proceed with the quotation.

5. **Postback URL Configuration**:
   - The temporary postback URL provided is only for initial testing. The client must configure and provide their own postback URL for production use. This can lead to issues if not properly set up before the bot is deployed.

6. **JSON Structure Changes**:
   - Any changes in the required JSON structure or the addition of new health conditions and medications may necessitate updates to the bot's logic and configuration. Without these updates, the bot may not function correctly.

7. **Health Conditions and Medications Schema**:
   - Each health condition and medication requires a specific schema. Inconsistencies or errors in the schema provided can result in incorrect data submission or processing failures.

8. **Data Accuracy and Completeness**:
   - Ensuring the accuracy and completeness of the data provided in the JSON elements is crucial. Missing or incorrect data can lead to inaccurate quotations or failed submissions.

9. **Server Connectivity Issues**:
   - Any connectivity issues between the bot and the Insurance Toolkit servers can disrupt the quotation process, leading to delays or failed requests.

10. **System Maintenance and Updates**:
    - Regular maintenance and updates of both the bot system and the Insurance Toolkit platform are necessary to ensure continued compatibility and optimal performance. Neglecting these updates can lead to system failures or degraded performance.

11. **Dependence on HTML and CSS Structure**:
    - The bot system relies on the HTML and CSS structure of the Insurance Toolkit host. If any changes occur in these structures, such as during a UI update on the host, the system may break. In such cases, all references to XPATHs and CSS Selectors must be rewritten to restore functionality.

12. **Headless Mode Operation**:
    - The bot must run in headless mode as the preferred option. Running in graphical mode demands more processing resources and is only recommended for maintenance, presentation, and development purposes. In live mode, headless operation is by far the best option for optimal performance and efficiency.
