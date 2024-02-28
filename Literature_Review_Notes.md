# Notes from the various research articles used for this project:

## Data modality fusion techniques

## Deep learning xAI methods applicable to survival analysis

## Survival analysis methods with a focus on hazard functions within the medical domain. 

Introduction to Survival Analysis in practice: 
    - An introduction to survival models including the Cox proportional hazard model. Gives several theoretical outlines and works through multiple sets of equations to give an overview of intuition behind the theory, including addition mathematics for situations that are less 'perfect' and closer to practice, like when the PH assumption does not hold, or covariates cannot be assumed to be discrete. A few methods for dealing with ties (two events share the same time interval) in the discrete data is also discussed.

Cox regression survival analysis with compositional covariates:
    - Presents a new framework for incorporating compositional covariates to the hazard model by using log-ratio coordinates to better balance the composition internal to composited covariates, allowing for better modeling of things like physical exercise and nutrition.

Ingoring competing events in the analysis of survival data may lead to biased results:
    - The researchers show that the use of censoring individuals of competing events will skew results if not properly accounted for.

Information criteria for detecting change-points in Cox hazard models:
    - 