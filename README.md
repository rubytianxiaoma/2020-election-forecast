# Overview

This repo contains code and data for forecasting the US 2020 presidential election. It was created by Boyu Sheng, Jiaxiang Miao, Qiyue Zhang, TianXiao Ma. The purpose is to create a report that summarises the results of a multilevel model that we built. Some data is unable to be shared publicly. We detail how to get that below. The sections of this repo are:  clean data script and output.

Clean data script folder contains code that modify the Nationscape survey(Individual survey data) and the ACS 2018(Post-stratification data), and the code that build the report paper.

The original dataset is obtained from :

- Democracy Fund + UCLA Nationscape survey results released on June 25th , 2020 is the individual survey level data used in the paper. 
Tausanovitch, Chris and Lynn Vavreck. 2020. Democracy Fund + UCLA Nationscape, October 10-17, 2019 (version 20200814). Retrieved from https://www.voterstudygroup.org/downloads?key=84a68f37-86ac-4871-b68a-a57b4d9e31d2
The report uses Nationscape wave 50 survey result. Original file can be downloaded by first requesting dataset from Democracy Fund Voter Study Group, clicking 'Download the .dta files' through the link send to the email. Then click 'phase_2_v20200814', open 'ns20200625' and find 'ns20200625.dta'. Or readers can simply use the /Output/survey.csv in the repo.
  Corresponding cleaning code modified from the Nationscape survey is:
  - clean_survey_data.Rmd

- 2018 American Community Survey is the Post-stratification dataset used in the paper.
Steven Ruggles, Sarah Flood, Ronald Goeken, Josiah Grover, Erin Meyer, Jose Pacas and Matthew Sobek. IPUMS USA: Version 10.0 [dataset]. Minneapolis, MN: IPUMS, 2020.
https://doi.org/10.18128/D010.V10.0
If the reader is interested in getting original dataset, please first register with IPUMS USA, then Get data, select 2018 ACS, select variables 'educ','sex','hispan','stateicp','age','race', then download a data extract. Or readers can simply use the /Output/cell_post.csv in the repo.
  Corresponding cleaning code modified from the 2018 ACS survey in the clean data script folder:
  - clean_ACS2018_data.Rmd

- Bidengo.Rmd contains code build for the report paper,paper can be found in the repo locates at /Paper/Bidengo.pdf.

Output folder contains data that are modified from the two original datasets, Code can be found in clean data script folder: Bidengo.Rmd

- survey.csv, modified from the Democracy Fund + UCLA Nationscape project.
- cell_post.csv, modified from ACS data

Paper folder contains the report that are modified from output data. Corresponding code script can be found in Clean data script folder. 

- Bidengo.pdf