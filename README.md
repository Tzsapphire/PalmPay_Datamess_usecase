# PalmPay_Datamess_usecase
Analysing Palmpay data mess 

The previous data structure  has a lot of discrepancies of tables viewed by the each team : operations, finance team.
In my new architecture, we wil be bringing the data together into a single AWS database - this will make sure that all teams are reading updated tables. 
Next the transformations will be done to create cleaned tables for the teams and it will be updated regularly through orchestration. the transformations done will also be version controlled with git, for ease of update and change. I suggest using dbt for these transformations for easy documentation.