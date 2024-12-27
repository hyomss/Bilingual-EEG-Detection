# Bilingual-EEG-Detection  
Excited to share my recent experience participating in the Sandia Lab Datathon! 🎉  

This project aimed to detect bilingual participants by analyzing N400 reactions in EEG data.  
Using a dataset of over 20,000 observations (spanning 600 word combinations across 40 participants) and leveraging 256 time frames recorded from 30 channels, I explored the fascinating intersection of neuroscience and machine learning.

####  Highlights of the dataset:

- Prime and target word pairs in four languages (English, Spanish, French, German)    
- Electrode readings from -100ms to 900ms  
- N400 response as the key signal, observed at 0ms post-target word display   

I used two methods for this project: time series k-means clustering and a 1D Convolutional Neural Network.  

For time series clustering, I first preprocessed the EEG data by centering it to zero and reducing noise using a simple natural cubic spline.   
Although EEG data often contains significant noise, it also includes critical spikes. Smoothing the data did not perform well in this context, and the second method, the CNN model, outperformed clustering in terms of accuracy. The computational environment was a basic Jupyter Notebook, and the CNN model took about 5 minutes to run.  
 
This Datathon was graded on a 20-point scale, and my presentation and code earned 11 points—just 3.75 points behind the winning team—all while competing solo!  
It was an incredible experience working with biological data, exploring the potential applications of EEG data, and discovering key factors within the dataset.
