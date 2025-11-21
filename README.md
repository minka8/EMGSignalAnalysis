# EMG Signal Analysis

This project contains a full analysis of electromyography (EMG) signals collected through custom experiments. The goal is to preprocess, visualize, filter, and extract meaningful information from EMG recordings obtained from different participants and experimental conditions.

---

## Dataset Description

The signals come from two experimental sessions:

- **Experiment 1** – Maximum voluntary contraction (MVC) measurements  
  File format: `MVK_IDn.txt`

- **Experiment 2** – EMG data during repeated muscle activations  
  File format: `eksperiment2_IDn.txt`

Each file contains raw EMG values sampled at:

- **Sampling frequency:** 1000 Hz  
- **IDs:** 1–7 (different subjects or sessions)

The notebook allows selecting the dataset by changing the `ID` parameter.

---

## Project Workflow

The notebook performs the following steps:

### **1. Importing Libraries**
NumPy, Pandas, Matplotlib, and SciPy are used for:
- Signal manipulation  
- Numerical processing  
- Filtering  
- Visualization  

### **2. Signal Visualization**
Raw EMG signals are plotted to inspect:
- Noise levels  
- Bursts of activity  
- Overall waveform characteristics  

### **3. Filtering EMG Signals**
Filtering includes:
- High-pass / low-pass filtering  
- Notch filters (if needed)  
- Smoothing  
- Envelope detection  

SciPy’s `signal` module is used for implementing digital filters.

### **4. Signal Processing**
Common EMG processing steps include:
- Rectification  
- RMS window calculation  
- Envelope extraction  
- Comparison of MVC vs. activation signals  

### **5. Interpretation**
The notebook allows comparisons between multiple IDs and experimental sessions to analyze muscle activation behavior.

---

