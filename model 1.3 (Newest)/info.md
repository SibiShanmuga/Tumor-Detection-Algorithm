This is the most upto date model of the tumor detection model.

**Updates**

- Improved confusion matrix
    - Tuned class weights
        -Punishes class 1 more
            Improves recall
            
- Improved learning speed
    - Higher learning rate at earlier epochs
    - Lower learning rate at later epochs
    - Trains general concepts faster

- Learning rate now reduces with each restart
 
**Issues**
There are no known major issues. Although there are a few minor issues that will be addressed in the future

According to the confusion matrix
- Class 1 (meningioma) gets slightly confused with Class 2 (notumor)
    Will try increasing augmentation
    
**Results**
I have found my best metrics so far, and have hit a major milestone!
*Note: These results are from held out testing data that have not been used in training or validation to uphold the integrity of the scores**

Accuracy: 95.65%
Loss: 0.3110
