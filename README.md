# Bilingual-EEG-Detection  
Excited to share my recent experience participating in the Sandia Lab Datathon! 🎉  

This project aimed to detect bilingual participants by analyzing N400 reactions in EEG data.  
Using a dataset of over 20,000 observations (spanning 600 word combinations across 40 participants) and leveraging 256 time frames recorded from 30 channels, I explored the fascinating intersection of neuroscience and machine learning.

####  Highlights of the dataset:
- Prime and target word pairs in four languages (English, Spanish, French, German)    
- Electrode readings from -100ms to 900ms  
- N400 response as the key signal, observed at 0ms post-target word display

#### EEG channel selection:
In this datathon project, I initially analyzed EEG data using the Cz electrode, referencing previous studies that highlighted its relevance to motor and sensory processing. However, considering the Pz electrode's stronger association with higher-level cognitive functions such as attention, memory, and semantic processing, including its role in capturing the N400 component during language comprehension, I hypothesized that Pz data might yield more relevant insights. To validate this, I compared the results from both electrodes to assess their effectiveness in reflecting the underlying neural processes.  

#### Model selection:
I used two methods for this project, time series k-means clustering and a 1D Convolutional Neural Network.  

For time series clustering, I first preprocessed the EEG data by centering it to zero and reducing noise using a simple natural cubic spline. Although EEG data often contains significant noise, it also includes critical spikes. Smoothing the data did not perform well in this context.   
CNN model is well-suited for capturing local patterns in EEG data, effectively learning features like the N400 effect within specific time intervals. 1D CNN model outperformed clustering in terms of accuracy.  
The computational environment was a basic Jupyter Notebook, and the CNN model took about 5 minutes to run.  
 
This Datathon was graded on a 15-point scale, and my presentation and code earned 11 points—just 3.75 points behind the winning team—all while competing solo!  
It was an incredible experience working with biological data, exploring the potential applications of EEG data, and discovering key factors within the dataset.
