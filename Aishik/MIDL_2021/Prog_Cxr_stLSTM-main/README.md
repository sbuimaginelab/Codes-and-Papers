# Prog_Cxr_stLSTM
Code for paper "Prediction of COVID-19 Lung Infiltrate Progression on Chest Radiographs Using Spatio-temporal LSTM based  Encoder-Decoder Network", accepted in MIDL 2021 [[paper]](https://openreview.net/pdf?id=96BhL_MERil) 

Aishik Konwer, Joseph Bae, Gagandeep Singh, Rishabh Gattu, Syed Ali, Jeremy Green, Tej Phatak, Amit Gupta, Chao Chen, Joel Saltz, Prateek Prasanna

## Abstract
Automated analyses of chest imaging in Coronavirus Disease 2019 (COVID-19) have largely focused on a single timepoint, usually at disease presentation, and have not explicitly taken into account temporal disease manifestations. We present a deep learning-based approach for prediction of imaging progression from serial chest radiographs (CXRs) of COVID-19 patients. Our method first utilizes convolutional neural networks (CNNs) for feature extraction from patches within the concerned lung zone, and also from neighboring areas to enhance the contextual phenotypic information. The framework further incorporates two distinct spatio-temporal Long Short Term Memory (LSTM) modules for effective predictions. The first LSTM module captures spatial dependencies between patches and the second exploits the temporal context of sequential CXR scans. The resulting network focuses on critical image regions that provide relevant information for learning the progression of lung infiltrates without the explicit need for infiltrate segmentation. The second LSTM provides an encoded context vector used as an input to a decoder module to predict future severity grades. Our novel multi-institutional dataset comprises sequential CXR scans from N=100 patients. Specifically, our framework predicts zone-wise disease severity for a patient on the last day by learning representations from the previous temporal CXRs. We design two baseline approaches - one using fine-tuned VGG-16 features and the other using radiomic descriptors. Experimental results demonstrate that our proposed approach outperforms both baselines in average accuracy by 10.33\% and 12.16\%, respectively, in predicting COVID-19 progression severity.

