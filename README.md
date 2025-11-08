# VMD And CNN-BiLSTM for Classification of Barbell Exercises

We utilize publicly available Barbell Exercise Tracking IMU dataset containing accelerometer and gyroscope measurements from from a single wrist-worn IMU while five participants performed various exercises including bench press (bench), squat, overhead press (ohp), row and deadlift(dead).The data collection occurs at 12.5 Hz for Accelerometer and 25 Hz for Gyroscope.The dataset comprises several csv files where each file corresponds to a particular exercise, participant and either accelerometer or gyroscope measurements with a unique time stamp </br></br>
The Detailed Code  is available here: https://www.kaggle.com/code/vish908/gym-exercise-classification
</br>
</br>
🌈 Step 1: Data Processing


&nbsp;&nbsp;&nbsp; ✨ Read accelerometer and gyroscope data

&nbsp;&nbsp;&nbsp; ✨ Create required dataframe columns such as participant, label and category

&nbsp;&nbsp;&nbsp; ✨ Merge the accelerometer data and gyroscope data

&nbsp;&nbsp;&nbsp; ✨ Resample the merged data

&nbsp;&nbsp;&nbsp; ✨ Export the preprocessed data

</br>
🌈 Step 2 : Visualize </br></br>
      ✨ Visualizing different types of exercise based on category or participant
</br>
</br>
</br>
🌈 Step 3: Outlier detection
</br>
</br>        

&nbsp;&nbsp;&nbsp;✨ Defining the three different methods for outlier detection 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.Interquartile range

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2.Chauvenet's criterion 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3.Local Outlier Factor 

</br>

🌈 Step 4: Feature Engineering


&nbsp;&nbsp;&nbsp; 📚 4.1 : Handling outliers - Interpolation

&nbsp;&nbsp;&nbsp; 📚 4.2 : Reduce noise/smoothing data - Kalman filter vs Butter worth low pass filter

&nbsp;&nbsp;&nbsp; 📚 4.3 : Reduce dimensionality of datasets - Principal component Analysis

&nbsp;&nbsp;&nbsp; 📚 4.4 : Qunatify model variability/Model optimization - Sum of sqaures attribute

&nbsp;&nbsp;&nbsp; 📚 4.5 : Temporal Abstraction - Rolling mean

&nbsp;&nbsp;&nbsp; 📚 4.6 : Frequency Abstraction - Variational Mode Decomposition vs Fourier transformation

&nbsp;&nbsp;&nbsp; 📚 4.7 : Resolve overlapping windows

</br>

🌈 Step 5 : Predictive modelling


&nbsp;&nbsp;&nbsp; ✨ Split features into different subsets
  
&nbsp;&nbsp;&nbsp; ✨ Carry out forward feature selection utilizing decision tree and identify the best 10 features and their scores
  
&nbsp;&nbsp;&nbsp; ✨ Grid search Across different machine learning Approaches 
</br>
  </br>

🌈 Step 6: Model Evaluation and Validation

&nbsp;&nbsp;&nbsp; ✨ Analyzed misclassifications to identify patterns of error and refine the model

&nbsp;&nbsp;&nbsp; ✨ Visualization of training/validation loss curves and class-specific performance helped detect overfitting 

&nbsp;&nbsp;&nbsp; ✨ Finally, I compared the CNN + BiLSTM model against other approaches, demonstrating the advantage of modeling both spatial and </br></br>
            temporal dependencies for high-fidelity exercise classification
</br>
