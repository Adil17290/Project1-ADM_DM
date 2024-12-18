# MSDS Admission Model for Decision Making (ADM-DM)

**Empowering Smarter Decisions with Data-Driven Insights for MSDS Admissions**

## Overview
The ADM-DM project is an innovative solution designed to streamline university admissions by automating transcript data extraction and GPA prediction. This system integrates Optical Character Recognition (OCR) with predictive modeling to process academic transcripts and calculate GPAs efficiently, accurately, and at scale.

## Key Features
- **Automated Transcript Processing**: Real-time extraction of data from academic transcripts in diverse formats (PDF, JPEG, PNG).
- **GPA Prediction**: Uses a Random Forest model for accurate and consistent GPA predictions.
- **User-Friendly GUI**: Simplifies interaction by allowing users to upload transcripts and receive GPA predictions seamlessly.
- **Scalability and Fairness**: Designed for high-volume processing with fairness checks to ensure unbiased results.

## Methodology
1. **Data Collection**: Transcripts were collected and annotated using PPOCRLabel.
2. **Preprocessing**: 
   - Conversion of transcripts into JSON files.
   - Super-resolution techniques applied for enhanced OCR accuracy.
3. **OCR Development**:
   - Fine-tuned PaddleOCR pretrained models to handle diverse transcript formats.
4. **Post-Processing**:
   - Structured extracted data into a tabular format for easy analysis.
5. **GPA Prediction**:
   - Leveraged Random Forest models with weighted grade calculations.
6. **GUI Integration**:
   - Unified application for data upload, processing, and GPA prediction.

## Model Accuracy
| Task          | Precision | Recall | F1-Score |
|---------------|-----------|--------|----------|
| Text Detection| 0.98      | 0.95   | 0.97     |
| Text Recognition| 0.96   | 0.98   | 0.95     |

## Deployment
- Local GUI application for offline processing of transcripts.
- All processing, including OCR and GPA prediction, occurs on the user's machine to ensure privacy and fast results.

## Challenges and Solutions
- **Data Quality**: Enhanced low-resolution images using super-resolution techniques.
- **Scalability**: Implemented modular architecture to support parallel processing.
- **Fairness**: Standardized GPA calculations and fairness checks for unbiased results.

## Deliverables
1. Annotated dataset for OCR training.
2. Enhanced OCR models with fine-tuning and preprocessing.
3. GUI application for streamlined transcript analysis and GPA prediction.

## Future Work
- **Multilingual OCR**: Extend support for non-English transcripts.
- **Scholarship Prediction**: Analyze student data to predict eligibility for scholarships.
- **API Integration**: Seamlessly integrate with existing admission platforms.
- **Predictive Course Planning**: Personalized course recommendations based on academic history.

## Lessons Learned
- Importance of robust preprocessing for noisy datasets.
- Value of iterative testing across diverse transcript formats.

## Conclusion
The ADM-DM project sets a benchmark in automating academic data management, enhancing the efficiency and fairness of university admissions. Future developments will include multilingual support and advanced analytics for broader applicability and impact.

---

**Contributors**: Shaik Adil, Pulleti Charan Sumanth, Bhonagiri Sruthi, Vemireddy Navya, Talasani Snithika Patel, Dacharla Sai Kumar, Tumma Karthik Reddy, Anabathula Deepa, Gembali Kalkesh.
