# fitness_track_model
Development of fitness track model for Hackathon AI Mathworks 2024 Thessaloniki
Participants: Vasilis Tsioulos

# Goal of this work!
The goal of this work is to take the datasets that the mathworks provided as examples in the repository [matlab-mobile-fitness-tracker](https://github.com/mathworks/matlab-mobile-fitness-tracker) and perform Data analysis techniques in order to check the validity of the examples
> Disclaimer : The data used in this case are NOT as valid as the data that one can extract by him/herself using matlab mobile!
# Code Structure
## Functions
1. AugmentWithNoise
2. AugmentWithNoisePosition
2 similar functions were created due to the different shape of the position matrix
## Data Preprocessing
The data were preprocessed with augmentation and concatenation between the augmented datasets
## Data Visualization
The plots that were created were:
* 3 scatter 3dplots for the (Sit activity, Walk aactivity and Run activity)
* 1 scatter 3dplot of the longitude and latitude (Position)
The plots were made by the augmented datasets in order to visualize the data and check if we could perform some more analysis
## Model Development
1. Compute the time that the person runs
2. compute the velocity of x y z
3. compute the distance traveled
4. if the threshold time is more than the running time it ouputs 0, else it outputs 1. 0 and 1 are used to remind the person to rest (1)
5. Compute the mean and std in order to has some insights
6. Normalization of the data
2 models were used
1. Random Forest classification
2. Logistic regression model
# Results
The models had 100% accuracy, that alone can be enough information to see that there's a high probability of overfitting. The 2 models were picked in order to have a regression and a classification method and they validated that the results are indeed overfitting. In real world applications and data, the model "cannot" achieve 100% accuracy but can go really close. That indicates that there are may be errors in the code or inaccurate and chaotic data that the model cannot capture their pattern.  
