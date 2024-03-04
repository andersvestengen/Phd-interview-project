# Notes from the various research articles used for this project:

## Data modality fusion techniques

## Deep learning xAI methods applicable to survival analysis

## Survival analysis methods with a focus on hazard functions within the medical domain. 

Introduction to Survival Analysis in practice: 
    - An introduction to survival models including the Cox proportional hazard model. Gives several theoretical outlines and works through multiple sets of equations to give an overview of intuition behind the theory, including addition mathematics for situations that are less 'perfect' and closer to practice, like when the PH assumption does not hold, or covariates cannot be assumed to be discrete. A few methods for dealing with ties (two events share the same time interval) in the discrete data is also discussed.

### Ranking the different Paper's model performance:
    1. PC-Hazard
    2. DeepHit
    3. Cox-Time
    4. Nnet-survival
    5. DeepSurv
    6. N-MTLR
    7. MTLR

### Ranking Modality fusion paper propositions: (Results and Practicality)

    1. Lung cancer paper            (CT & clinical data)                    (.885 acc.,  .957  AUROC , 2022) 
    2. Pulmonary elmbolism (Nature) (CT & clinic data EMR)                  (.885 acc.,  .947  AUROC , 2020)  
    3. Babies paper                 (CTG and clinical information (sparse)) (.907 acc.,  .920  AUC   , 2023)        (Check out LGBM classifier)
    4. Skin Lesion smartphone       (clinical images & clinical data)       (.760 acc.,  .947  AUROC , 2022) 
    5. Stroke paper                 (MRI & clinical data)                   (.804 acc.,  .870  AUC   , 2024)
    6. ICU paper                    (X-ray & clinical data)                 (.770 acc.,  .770  AUC   , 2023)


### Ranking of the different xAI propositions: (Results and Practicality)




# Proposition for the complete model

## Desc. "A multimodal explainable deep learning method for predicting survival probabilities of individual liver cancer patients by integrating information from CT and clinical parameters"

### What Survival function should be used?
    PC-Hazard seems to score the best of the surveyed models, but I've not yet considered the actual task of liver cancer patients. (DeepHit could be a better fit)

### What xAI method should be used?
    

### What modality fusion technique should be used?