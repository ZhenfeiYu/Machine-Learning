# Machine-Learning
## Supervised Learning
### KNN
#### Definiation
k<=20 if the majority of k nearest sample data belongs to one class, the sample data can be classified into this class. The neighbors are correctly classified(labeled).  
优势：欧式距离  
     KNN通过依据k个对象中占优的类别进行决策，而不是单一的对象类别决策  
NN classifier: training data (x1,y1)...(xm,ym), xi be the point x1...xm closest to x return yi.  
K-NN classifier: training data (x1,y1)...(xm,ym)  
Construct function as:  
Xi1, xi2,...xik be the k points among x1, x2,... xm that are closest to   
Return the majority of labels of yi1, yi2...yik  
#### Procedure:  
1. Load data  
2. Initialize the value of k
3. Iterate from 1 to k trained data points (neighbors):  
   Calculate the distance of test data and each training data, using euclidean distance.    Sort the distances in ascending order.  
   Get top k rows  
   Get the moset frequent class  
   Return predicted class  

#### Effect of k:  
smaller k => smaller training error  
Larger k => predictions are more stable due to voting  
The boundary becomes smoother with the increase of k  
#### Choice of k:  
Minimize the validation error  
Minimize loocv error  

python实现
