************************************************************************************************************************
The given folder contains all the codes required, but the data set folders have to be added IN THE SAME FOLDER as that of the codes
To create such folder:
	Keep all 4 code files in a folder. Keep the HMM-Code folder ,data set folders in this same folder (files that had to be added in our case was "bA,chA,dA,IA,tA,HMM-CODE" + the 4 .py files that are in the folder)

dtwtel.py runs DTW on Telugu Characters
hmmtel.py runs HMM on Telugu Characters 
To compare ROC_DET curves for these two, first run dtwtel.py, then uncomment last part in hmmtel.py and run it

Note that DTW takes long time to run, it produces the confusion matrix and ROC,DET curves and prints Accuracy.
HMM runs quicker, still takes a while because of the custom KMeans function used instead of the inbuilt Kmeans functions.
HMM codes give out, Confusion matrices and ROC,DET curves for each of the cases. IGnore Prints
Last PRINT gives accuracies

************************************************************************************************************************

File structure for running th files:
Current folder has the codes.
Put Telugu datasets in the current folder.(Names: bA,chA,dA,lA,tA)

LR.py performs Logistic Regression, with PCA,LDA, stores some ROC values in a file called rocvals.txt. Outputs required accuracies and graphs onto stdout.

KNN_SVM_ANN.py does the remaining tasks. It also prints accuracies and graphs to stdout. It additionally expects a rocvals.txt file to plot ROCs of LR along with KNN,SVM,ANN.

To run		--> python3 LR.py
Next run     	--> python3 KNN_SVM_ANN.py

************************************************************************************************************************

