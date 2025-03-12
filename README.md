# Deep Learning
The use of a Deep Neural Network (DNN) in cybersecurity is a new research interest for many cybersecurity professionals, and a deep neural network for IDS is one such research area. This is because the DNNs have the capabilities to manage enormous data that helps them to have a better performance in classification than the traditional machine learning techniques, which previously have shown to be a stronger and better defense mechanism over the signature-based intrusion detection systems.

### Objective
The goal of this thesis work is to create and analyze a deeper machine learning technique using a deep neural network that can 
be implemented on a signature or an anomalous behaviour of network traffic. 
### Results Analysis and Discussion 
In this thesis, the researcher has conducted a comparative study of the machine learning approaches for intrusion detection using conventional machine learning algorithms and feedforward deep neural networks (FFDNN). My main idea was to develop an FFDNN as a 
classifier to classify network traffic intrusions in the NSL-KDD dataset as normal or attack while using the conventional machine learning approaches as my controlled experiment. The analysis was performed on five different ML algorithms (DT, LR, RF, NB, KNN) and their performances on the test data gave 81%, 76%, 77%, 77%, 77% respectively. 

I also analysed three different FFDNNs, namely FFDNN-1, FFDNN-2, FFDNN-3 based on different hyperparameter values, feature reduction, and data encoding techniques. Their performances on the test data are 89%, 84%, and 87% respectively. Some important performance indicators, namely, accuracy, true positive rate (TPR = recall), false-positive rate (FPR), precision, F1 measure, and ROC area under the curve (AUC) are used as the bases to judge the model's performance.

![image](https://github.com/user-attachments/assets/5804b98d-e284-4ce2-9084-12bc64e3c93f)

![image](https://github.com/user-attachments/assets/cc1585c2-23f2-4677-979f-b1e169acc652)

![image](https://github.com/user-attachments/assets/98d06605-e840-4f02-8b62-93650c08bbdc)

Considering overall performances of all models, the FFDNN-1 performed best with the highest detection accuracy of 89% and precision of 91%, however, the precisions of the DT, RF, and NB were quite high even though their detection accuracy was not above 80% except DT that gave 81%. High precision indicates that the models are reliable compared to low precision, which can result in a lot of false positives as in the case of the KNN classifier. Another point to note is that high recall does not necessarily mean the best performance, but rather higher F1-measure shows that the model had performed very well. This is because the F1 measure takes into account the harmonic mean of precision and recall, so it tells how accurate a model is. From the results shown in Table 17, FFDNN-1 had an F1-measure of 90%, which makes it the best model, other FFDNN variants also had a high F1-measure when compared to the F1-measure of the conventional machine learning algorithms. 

Another important metric that shows that the FFDNNs performed well is their high ROC area under the curve (AUC), FFDNN-1, FFDDN-2, and FFDNN-3 in Table 16 all had values of 95%, 86%, and 92% in that order. The higher the AUC value, the more optimal the model becomes (note that 100% indicates a perfect model). Also, it is good to know that the primary aim is to develop machine learning models that would maintain an acceptable true positive rate (TPR) or detection rate (DR) with low false alarm rate (FAR) or false positive rate (FPR), looking at Table 13 and Table 16, you could see that DT, RF, and NB had very low FAR of 5%, 3% and 2% respective compared to FFDNNs 11%, 16%, and 13%. This is good even though their detection rates were not as high as the FFDNNs, however, there could still be an improvement in ensuring that the FFDNNs produce low FAR since they are scalable in terms of architecture, but this would involve more computational cost. 

I would like to point out that any variant of the feedforward deep neural network (FFDNN-1, FFDNN-2, and FFDNN-3) has the capability as a classifier to classify network traffic intrusions with a high detection rate while offering a reduced FAR, it only depends on the model design, hyperparameters, and architecture. Limitations in the ML approach for intrusion detection are high FAR and how to strike a balance between false positive and false negative in terms of intrusion detection policies or profiling. I believe this limitation can be solved by the development of a deeper neural network or the use of another variant of a deep neural network like the convolutional deep neural network (CNN). 

