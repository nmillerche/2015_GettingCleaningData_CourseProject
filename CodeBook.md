#Code Book

## Study Design

###Data Set Information (from the UCI Machine Leraning Repository's "Human Activity Recognition Using Smartphones Data Set" https://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones):

"The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain."

The variables that were estimated from these signals are:

*  mean(): Mean value
*  std(): Standard deviation
*  mad(): Median absolute deviation 
*  max(): Largest value in array
*  min(): Smallest value in array
*  sma(): Signal magnitude area
*  energy(): Energy measure. Sum of the squares divided by the number of values. 
*  iqr(): Interquartile range 
*  entropy(): Signal entropy
*  arCoeff(): Autoregression coefficients with Burg order equal to 4
*  correlation(): Correlation coefficient between two signals
*  maxInds(): Index of the frequency component with largest magnitude
*  meanFreq(): Weighted average of the frequency components to obtain a mean frequency
*  skewness(): Skewness of the frequency domain signal 
*  kurtosis(): Kurtosis of the frequency domain signal 
*  bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT
   of each window.
*  angle(): Angle between some vectors.

No unit of measure is reported, as all variables were normalized and bounded within [-1,1].

##ID Fields

* `Subject` - The participant ID
* `ActivityId` - The label of the activity performed 

##Extracted Feature Names

* `TimeBodyAccelerometerMean()-X`                    
* `TimeBodyAccelerometerMean()-Y`                    
* `TimeBodyAccelerometerMean()-Z`                    
* `TimeBodyAccelerometerSTD()-X`                     
* `TimeBodyAccelerometerSTD()-Y`                     
* `TimeBodyAccelerometerSTD()-Z`                     
* `TimeGravityAccelerometerMean()-X`                 
* `TimeGravityAccelerometerMean()-Y`                 
* `TimeGravityAccelerometerMean()-Z`                 
* `TimeGravityAccelerometerSTD()-X`                  
* `TimeGravityAccelerometerSTD()-Y`                  
* `TimeGravityAccelerometerSTD()-Z`                  
* `TimeBodyAccelerometerJerkMean()-X`                
* `TimeBodyAccelerometerJerkMean()-Y`                
* `TimeBodyAccelerometerJerkMean()-Z`                
* `TimeBodyAccelerometerJerkSTD()-X`                 
* `TimeBodyAccelerometerJerkSTD()-Y`                 
* `TimeBodyAccelerometerJerkSTD()-Z`                 
* `TimeBodyGyroscopeMean()-X`                        
* `TimeBodyGyroscopeMean()-Y`                        
* `TimeBodyGyroscopeMean()-Z`                        
* `TimeBodyGyroscopeSTD()-X`                         
* `TimeBodyGyroscopeSTD()-Y`                         
* `TimeBodyGyroscopeSTD()-Z`                         
* `TimeBodyGyroscopeJerkMean()-X`                    
* `TimeBodyGyroscopeJerkMean()-Y`                    
* `TimeBodyGyroscopeJerkMean()-Z`                    
* `TimeBodyGyroscopeJerkSTD()-X`                     
* `TimeBodyGyroscopeJerkSTD()-Y`                     
* `TimeBodyGyroscopeJerkSTD()-Z`                     
* `TimeBodyAccelerometerMagnitudeMean()`             
* `TimeBodyAccelerometerMagnitudeSTD()`              
* `TimeGravityAccelerometerMagnitudeMean()`          
* `TimeGravityAccelerometerMagnitudeSTD()`           
* `TimeBodyAccelerometerJerkMagnitudeMean()`         
* `TimeBodyAccelerometerJerkMagnitudeSTD()`          
* `TimeBodyGyroscopeMagnitudeMean()`                 
* `TimeBodyGyroscopeMagnitudeSTD()`                  
* `TimeBodyGyroscopeJerkMagnitudeMean()`             
* `TimeBodyGyroscopeJerkMagnitudeSTD()`              
* `FrequencyBodyAccelerometerMean()-X`               
* `FrequencyBodyAccelerometerMean()-Y`               
* `FrequencyBodyAccelerometerMean()-Z`               
* `FrequencyBodyAccelerometerSTD()-X`                
* `FrequencyBodyAccelerometerSTD()-Y`                
* `FrequencyBodyAccelerometerSTD()-Z`                
* `FrequencyBodyAccelerometerMeanFreq()-X`           
* `FrequencyBodyAccelerometerMeanFreq()-Y`           
* `FrequencyBodyAccelerometerMeanFreq()-Z`           
* `FrequencyBodyAccelerometerJerkMean()-X`           
* `FrequencyBodyAccelerometerJerkMean()-Y`           
* `FrequencyBodyAccelerometerJerkMean()-Z`           
* `FrequencyBodyAccelerometerJerkSTD()-X`            
* `FrequencyBodyAccelerometerJerkSTD()-Y`            
* `FrequencyBodyAccelerometerJerkSTD()-Z`            
* `FrequencyBodyAccelerometerJerkMeanFreq()-X`       
* `FrequencyBodyAccelerometerJerkMeanFreq()-Y`       
* `FrequencyBodyAccelerometerJerkMeanFreq()-Z`       
* `FrequencyBodyGyroscopeMean()-X`                   
* `FrequencyBodyGyroscopeMean()-Y`                   
* `FrequencyBodyGyroscopeMean()-Z`                   
* `FrequencyBodyGyroscopeSTD()-X`                    
* `FrequencyBodyGyroscopeSTD()-Y`                    
* `FrequencyBodyGyroscopeSTD()-Z`                    
* `FrequencyBodyGyroscopeMeanFreq()-X`               
* `FrequencyBodyGyroscopeMeanFreq()-Y`               
* `FrequencyBodyGyroscopeMeanFreq()-Z`               
* `FrequencyBodyAccelerometerMagnitudeMean()`        
* `FrequencyBodyAccelerometerMagnitudeSTD()`         
* `FrequencyBodyAccelerometerMagnitudeMeanFreq()`    
* `FrequencyBodyAccelerometerJerkMagnitudeMean()`    
* `FrequencyBodyAccelerometerJerkMagnitudeSTD()`     
* `FrequencyBodyAccelerometerJerkMagnitudeMeanFreq()`
* `FrequencyBodyGyroscopeMagnitudeMean()`            
* `FrequencyBodyGyroscopeMagnitudeSTD()`             
* `FrequencyBodyGyroscopeMagnitudeMeanFreq()`        
* `FrequencyBodyGyroscopeJerkMagnitudeMean()`        
* `FrequencyBodyGyroscopeJerkMagnitudeSTD()`         
* `FrequencyBodyGyroscopeJerkMagnitudeMeanFreq()`    
* `Angle(TimeBodyAccelerometerMean,Gravity)`         
* `Angle(TimeBodyAccelerometerJerkMean),GravityMean)`
* `Angle(TimeBodyGyroscopeMean,GravityMean)`         
* `Angle(TimeBodyGyroscopeJerkMean,GravityMean)`     
* `Angle(X,GravityMean)`                             
* `Angle(Y,GravityMean)`                             
* `Angle(Z,GravityMean)`                             
* `Subject`                                          
* `ActivityId`

## Activity Labels

* `WALKING` (value `1`)
* `WALKING_UPSTAIRS` (value `2`)
* `WALKING_DOWNSTAIRS` (value `3`)
* `SITTING` (value `4`)
* `STANDING` (value `5`)
* `LAYING` (value `6`)
