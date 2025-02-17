# Speaker Recognition using Gaussian Mixture Models (GMM)

## Overview
This project focuses on **speaker recognition** using **Gaussian Mixture Models (GMM)**, a probabilistic model commonly used in speech processing for modeling the distribution of feature vectors extracted from audio signals. The goal is to build a system that can identify and verify speakers based on their unique voice characteristics.

## Objectives
- Preprocess and extract relevant features from audio recordings.
- Train Gaussian Mixture Models (GMM) for different speakers.
- Perform speaker identification and verification using GMM-based classification.
- Evaluate model performance and optimize parameters for better accuracy.

## Methodology

### 1. **Data Collection & Preprocessing**
- **Dataset**: Collected or used an existing dataset of recorded speech samples from multiple speakers.
- **Preprocessing**:
  - Converted audio files to a consistent format (e.g., `.wav`).
  - Removed noise using filtering techniques.
  - Extracted **Mel-Frequency Cepstral Coefficients (MFCCs)** as feature representations.

### 2. **Feature Extraction**
- Used **MFCC** features, which effectively capture timbral and phonetic characteristics of a speaker's voice.
- Extracted features using **Librosa** or **Python SpeechRecognition libraries**.

### 3. **Modeling with GMM**
- Trained a separate **GMM** for each speaker using the extracted MFCC features.
- Used **Expectation-Maximization (EM) algorithm** to estimate GMM parameters.
- Configured the number of Gaussian components based on speaker variability.

### 4. **Speaker Identification & Verification**
- **Identification**: Compared an unknown speaker’s MFCC features against trained models and assigned the most probable speaker.
- **Verification**: Compared a claimed speaker's voice against their trained model to confirm identity.

### 5. **Performance Evaluation**
- Measured system accuracy using **confusion matrix, precision, recall, and F1-score**.
- Analyzed the impact of different numbers of Gaussian components on recognition accuracy.

## Tools and Technologies
- **Programming Language**: Python
- **Libraries Used**:
  - `Librosa` (for feature extraction)
  - `SciPy` (for signal processing)
  - `Sklearn.mixture` (for GMM implementation)
  - `NumPy, Pandas` (for data handling)
  - `Matplotlib, Seaborn` (for visualization)

## Results and Findings
- Demonstrated successful speaker recognition with **GMM-based classification**.
- Found that **increasing Gaussian components improves accuracy up to a limit**.
- Identified **MFCCs as effective features** for speaker modeling.

## Future Improvements
- Integrate **Deep Learning models (e.g., GMM-HMM, CNNs, or LSTMs)** for improved accuracy.
- Expand the dataset with more speakers and diverse environmental conditions.
- Implement real-time speaker recognition using a **streaming audio framework**.

## Conclusion
This project successfully implemented **Speaker Recognition using GMM**, demonstrating the effectiveness of probabilistic modeling for voice-based authentication. It provides a foundation for **biometric security systems, voice assistants, and forensic applications**.

---
