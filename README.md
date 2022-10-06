# Credit_Risk_Analysis

## Overview 

### Purpose

The purpose of this analysis was to use machine learning to predict credit card risk; that is, we were to try and weed out the bad loans from the good. We were to use Oversampling, undersampling, SMOTEENN and random forest to accomplish this task. I chose random state 78 for anyone that would like to recreate my work.

## Results

### Resampling

#### Naive Random Oversampling

As you can see from the picture below, the accuracy of resampling tends to be middling to poor. This trend continued with all forms of the resampling, with none of the methods cracking 65%. However, the Naive Random Oversampling did have the highest accuracy score of all four methods.

<img width="505" alt="image" src="https://user-images.githubusercontent.com/105998378/194430652-f343e5b5-fdeb-45b4-a471-d018321d762b.png">

#### SMOTE Oversampling

Throughout the resampling the high risk category remained at 1%, meaning that the overwhelming majority of credit cards can be issued without fuss or worry.

<img width="494" alt="image" src="https://user-images.githubusercontent.com/105998378/194430709-12f1a384-ee03-47d3-adb0-9d62054595a2.png">

#### Undersampling

With undersampling we begin to see a slight rise in sensitivity, but only by 1%. Technically this would mean that undersampling performs better than oversampling, but because it's such a small amount better I can't make that declaration with any feeling of confidence.

<img width="490" alt="image" src="https://user-images.githubusercontent.com/105998378/194430763-ffd8cc71-a8fc-44ec-9f2b-dd62f0be6a6f.png">

#### Over/Under

The combination over/under-sampling model turned out to be the most sensitive, if the least accurate. None of the models showed consistently good sensitivity/accuracy combos.

<img width="491" alt="image" src="https://user-images.githubusercontent.com/105998378/194430788-d23f2972-f5ad-4b6c-aa66-7e2640e1a1fd.png">

### Ensemble

#### Balanced Forest

Right out of the gate we can see that balanced forest is much more accurate than any of the over/under samlping models, with a sensitivity almost rivaling that of the best performer for resampling, which is the combo over/under.

<img width="493" alt="image" src="https://user-images.githubusercontent.com/105998378/194427395-4e0d982f-99b0-4dc6-9b23-45282355b133.png">

#### Easy Ensemble

Better still is the Easy ensemble method of analysis. The accuracy was a whopping 92% with a sensitivity to match. This method blows all of the other methods out of the water, but we still see the same results; A high-risk category at only 1%.

<img width="509" alt="image" src="https://user-images.githubusercontent.com/105998378/194427248-591b52b3-cd98-4065-81a4-6e1e985fd78a.png">

## Conclusion

### Summary

In conclusion I would say that Easy Ensemble is the best method of them all and the one that I would recommend if someone were to ask me. The accuracy and sensitivity are both incredibly high without being so high as to make you think that it's over-fit. I would argue it's right on the cusp, but doesn't cross the line. I would also state that, based off of the results, you can safely issue credit cards to all but the worst credit offenders and that you will probably be fine. 
