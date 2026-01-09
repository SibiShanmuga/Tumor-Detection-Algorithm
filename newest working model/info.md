This is the most upto date model of the tumor detection model.

**Updates**
- Tuned the parameters to get better fitting
- Added a multi-run feature
  - If X epochs can't be hit in a single run it'll restart the run with the best model weights and the starting learning rate
 
**Issues**
There are a couple known issues that will be addressed in the upcoming update.
According to the confusion matrix,

- Class 1 (meningioma) is confused with Class 3 (pituitary) 49 times and Class 2 (no tumor) 21 times
  - Low recall

- Class 3 (pituitary) is over predicted causing false positives
  - Low precision
