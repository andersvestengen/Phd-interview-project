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




# Proposition for the complete model

## Desc. "A multimodal explainable deep learning method for predicting survival probabilities of individual liver cancer patients by integrating information from CT and clinical parameters"

### What Survival function should be used?
    PC-Hazard seems to score the best of the surveyed models, but I've not yet considered the actual task of liver cancer patients. (DeepHit could be a better fit)

### What xAI method should be used?
    

### What modality fusion technique should be used?