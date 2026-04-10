# PalmPay_Datamess_usecase
Analysing Palmpay data mess (from [PalmPay_Africa](https://datausecase.netlify.app/))

The previous data structure  has a lot of discrepancies of tables viewed by the each team : operations, finance team.
In my new architecture, we wil be bringing the data together into a single AWS database - this will make sure that all teams are reading updated tables. We are creating a AWSCloud data lake, so that we can have a single source of truth, and to protect against failures, so the lake has all the raw tables which you can always refer to incase of failures or break in pipeline.

Next the transformations will be done to create cleaned tables for the teams and it will be updated regularly through orchestration. the transformations done will also be version controlled with git, for ease of update and change. I suggest using dbt for these transformations for easy documentation.

 