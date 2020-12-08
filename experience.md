### Experience in  fMRI Software and Toolboxes, Deep Learning, and Machine Learning
```Neuroimaging```   ```MRI```   ```Nilearn```  ```CONN```  ```Big Data``` ```XGBoost```  ```Functional Connectivity```   ```Structural MRI```  ```Biomarker```
* **Neuroimaging biomarker detection for Schizophrenia and Autism Spectrum Disorder**
  * Objective was to detect the important biomarker for Schizophrenia and Autism Spectrum Disorder by employing the fMRI dataset from SchizConnect and ABIDE dataset.
  * Data preprocessing and further analysis were performed in the CONN toolbox in SPM, and a 4-D ROI mask was created using 2nd level analysis results.
  * ICA, PCA, and Dictionary learning analysis were further performed on the preprocessed dataset using GIFT toolbox and Nilearn, and a different 4-D mask was created.
  * Threshold region extractor was employed to extract time series of combined 4-D masks, and functional connectivity analysis was performed on the whole set of time series, and a 222*222 matrix was obtained.
  * Feature selection analysis was performed using XGBoost, and the features giving high classification accuracy between neuro-disorder class and healthy class on the test set are kept as our final feature matrix.
  * FreeSurfer analysis was performed on Structural MRI data; subcortical volume (48 features) and cortical region ROI's thickness (68 features) through Desikan-Killiany atlas were used as features.
  * Weighted Voting classifier was employed to achieve the best classification accuracy using functional final feature matrix and structural MRI features.
  * Features were projected back to obtain the biomarker for Schizophrenia and Autism Spectrum Disorder.
  * The sample code is available [here](https://github.com/Nitin-IITR/my-fmri_biomarker_detection/tree/master)
  
* **Optimized model for fMRI development data classification using Convolution Neural Network**
  * The project aimed to classify child (ages 3-12) and adult (ages 18-39) fMRI data, which can be obtained from [OpenNeuro](https://openneuro.org/datasets/ds000228/versions/1.0.0)
  * Smoothing of 2D slices of each 3-D functional image was performed using OpenCV.
  * Convolution neural network model was built through Keras to allow parallel computing using Cuda, and 2-D smoothed images were fed for classification.
  * An optimized model was further built with inbuilt smoothing and optimized classification without the need for any extra external storage for 2-D fMRI slices.
  * The code for optimized CNN model along with other models can be found [here](https://github.com/Nitin-IITR/fMRI-2D-Convolution)
  
* **Finger taping condition prediction through fMRI data**
  * The project's objective was to predict the subject's condition inside the fMRI scanner from finger tapping and rest condition. 
  * Preprocessing and full analysis was performed in SPM-12, and a 4-D ROI mask was created using 2nd level analysis results.
  * GIFT toolbox was employed for decomposition of fMRI data and the noise component were removed for further analysis.
  * Time series extraction was performed on both the mask and mean ICA mask after noise removal using threshold region extractor, and connectivity matrix was obtained by employing Nilearn analysis on time-series data.
  * Using the data points for each condition block, integration and mean features were extracted and used as a single datapoint for classification purposes.
  * SVM with the gaussian kernel was employed to classify these final obtained data after feature extraction, and high accuracy results were obtained.
  * Code for the above project can be found [here](https://github.com/Nitin-IITR/fMRI-finger_tapping)
  

### Experience on Signal processing, EEG, machine learning
```Signal processing```   ```EEG```  ```MNE```  ```Matlab```  ```Python```  ```Nolds```  ```Scikit-learn```
* **Physiological stress detection using EEG, ECG, and Pulse oximeter | Biomedical Instrumentation Lab IIT Roorkee**
  * Collected EEG, ECG, and Pulse oximeter data from the students at IIT Roorkee while performing physiological stress tasks (heavy exercise) followed by relaxation (breathing practice).
  * Employed statistical, entropy, and non-linear time series features and statistical tools like p-value and permutation test for optimal feature selection.
  * Implemented signal preprocessing and artifact removal using Discrete Wavelet Transform (DWT) algorithm, FIR bandpass filter, EEGIFT, and MNE tools
  * The technologies and libraries used were Python, Matlab, MNE, PyEEG, EEGIFT, Nolds, Scikit Learn, Scipy, Statistics.
  * *Note code will we public soon*
  

* **Epileptic seizure detection using EEG analysis | Biomedical Instrumentation Lab IIT Roorkee**
  * EEG signal analysis and feature extraction were performed to detect the onset of seizure activity and classify the EEG epilepsy Bonn dataset.
  * Signal processing was implemented using the Short-Time Fourier Transform (STFT) algorithm and MNE tools.
  * ANOVA, correlation matrix, and permutation test were employed to select the optimal feature matrix and obtained high accuracy results by applying machine learning techniques.
  * The research paper has also been communicated by Prof. on the project findings.
