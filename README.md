##  🧠 EEG-Based Emotion Recognition using DREAMER Dataset

An end-to-end neuroscience-driven machine learning system for decoding human emotions from EEG brain signals.

This project integrates signal processing, feature engineering, machine learning, and neural visualization into a scientifically validated affective computing pipeline.

🏆 Top 10 Finalist – IITM NeuroHack
## 📁 Project Structure

├── data/
├── preprocessing/
├── feature_engineering/
├── modeling/
├── visualization/
└── results/

📌 Project Overview

Human emotions shape the way we think, behave, and make decisions.
EEG signals capture brain activity linked to these emotions — but working with them isn’t easy. They are noisy, complex, and require careful scientific handling.

In this project, I built a complete end-to-end machine learning pipeline to classify emotional states from EEG signals using the DREAMER dataset.

This is not just a basic ML project — it combines neuroscience, signal processing, and machine learning into a structured, research-driven system.

✔ Scientific validation
✔ Signal preprocessing
✔ Feature engineering
✔ Machine learning modeling
✔ Neural visualization
✔ Real-world application focus

---

 🎯 Problem Statement

To design an EEG-based emotion recognition system that classifies emotional states using:

* Valence
* Arousal
* Dominance

With potential applications in:

🧠 Mental health monitoring
🤖 Emotion-aware AI systems
🚗 Driver drowsiness detection
🩺 Affective healthcare technologies

---

 📂 Dataset

**DREAMER Dataset (.mat format)**

* 18 participants
* 5 emotional stimuli
* Self-reported VAD emotional ratings
* EEG recorded using EMOTIV headset

---

🏗 Complete Project Pipeline

🔹 Phase 1: Emotional Structure Validation

* Loaded the DREAMER dataset
* Extracted Valence–Arousal–Dominance scores
* Computed stimulus-level averages
* Mapped emotions in the Arousal–Valence circumplex
* Verified correlations among V-A-D

✅ Confirmed dataset reliability for supervised learning

---

🔹 Phase 2: EEG Preprocessing

* 50 Hz Notch Filtering
* 0.5–45 Hz Band-pass Filtering
* Common Average Referencing (CAR)
* Independent Component Analysis (ICA)
* EMOTIV → 10–20 channel mapping

✅ Clean, artifact-free EEG signals ready for feature extraction

---

🔹 Phase 3: Feature Engineering

* Segmented EEG (baseline & stimulus)
* Power Spectral Density using Welch’s Method

Extracted frequency bands:

* Theta (4–8 Hz)

* Alpha (8–13 Hz)

* Beta (13–30 Hz)

* Gamma (30–45 Hz)

* Applied baseline correction

✅ Converted raw EEG into structured numerical feature vectors

---

🔹 Phase 4: Emotion Classification

* Converted VAD scores into binary classes
* Applied feature normalization
* Subject-aware train-test split (80:20)
* Trained SVM (RBF Kernel)

📊 Results:

* Accuracy: 0.75
* F1-score evaluated
* Confusion matrix analyzed

---

🔹 Phase 5: Visualization & Interpretation

* Class imbalance analysis
* Scalp Topographic Maps revealed:

  * Theta – Frontal activation
  * Alpha – Posterior patterns
  * Beta – Motor-related activity

These visualizations helped interpret spatial emotional signatures in the brain.

✅ Built an interpretable and application-ready affective computing system

---

💡 What Makes This Project Stand Out

✔ Complete end-to-end scientific pipeline
✔ Subject-aware validation (avoids data leakage)
✔ Interpretable neural band visualization
✔ Real-world application potential
✔ Strong integration of Neuroscience + Signal Processing + ML

---

## 🛠 Tools & Technologies

- Python
- NumPy
- Pandas
- MNE
- Scikit-learn
- Matplotlib
- SciPy

---

🏆 Achievement

Selected as **Top 10 Finalist at IITM NeuroHack**.

---

🔮 Future Scope

* Real-time EEG emotion detection
* Multi-modal emotion recognition
* Deep learning models (CNN / LSTM)
* Clinical mental health applications
  
🧠 EEG Preprocessing & Artifact Removal – Visual Evidence
🔹 Independent Component Analysis (ICA) – Spatial Components
  ![1](https://github.com/user-attachments/assets/1fc52800-6ccc-4306-b16d-4236f31c4e9d)
The ICA topographic maps show spatial distribution of independent components across the scalp.

✔ Identified eye-blink and muscle artifacts
✔ Separated neural vs non-neural activity
✔ Enabled precise artifact rejection


🔹 EEG Power Spectral Density (PSD)
![2](https://github.com/user-attachments/assets/ea7175bb-46d2-416f-89ea-e5cb6d332798)


Power Spectral Density analysis confirms:

✔ Clear physiological rhythms (0.5–45 Hz)
✔ Removal of 50 Hz power-line noise
✔ Proper band separation (Theta, Alpha, Beta, Gamma)

🔹 ICA Component Time-Series Signals
![3](https://github.com/user-attachments/assets/03595b2a-ef0b-4c00-b7db-b7f9bb63d445)


Time-domain visualization of ICA components:

✔ Detected blink-related spikes
✔ Removed high-amplitude muscle artifacts
✔ Preserved emotion-related neural oscillations






