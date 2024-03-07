## Notes from implementing survival functions on the Lung cancer set  

Want to implement the following solutions to compare
    - PC-Hazard (discrete)
    - DeepHit ()
    - Cox-time ()



Notes on the structure of the METABRIC dataset:
    - 9 covariates labeled x0,..,x8
    - Duration is regarded as right-censored event-time
    - events are labeled as 1 event, or 0 censored.


Where are the events for the Lung cancer dataset?
    - There doesn't seem to be any explicit event category. This wouldn't be so bad except there doesn't seem to be any distinction between event and censoring??

Notes from the summary study:
    - Patients with a 90-day mortality, or that had less than 24 months of follow-up were excluded. 
    - Any patient that received preoperative HAI were excluded.

    - From the description in the second sheet of the dataset, there seems to be three tables of events.
        1. overall survival yes/no
        2. Recurrence yes/no
        3. disease free survival
        4. Patient status for liver disease free survival (cancer is gone and patient is alive) yes/no. Censored either way?

    I would argue that in this case I don't care about the DFS-part of the statistics, only the overall survival-rate is important. 

        - There maybe a need to revisit and revise this, but for now the DFS columns will be removed (correlation would be absurd if they should remain?)

DFS vs OS analysis:
    - DFS can be seen as a competing risk versus 'Ordinary Survival', therefore separate analysis is prudent. So either use a competing-risk model, or do joint analysis. 

    - I should come back to this and check which of the survival models in my list is potentially capable of competing-risk or joint analysis. 
