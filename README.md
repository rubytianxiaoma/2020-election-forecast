# Overview

This repo contains code and data for forecasting the US 2020 presidential election. It was created by NAME. The purpose is to create a report that summarises the results of a multilevel model that we built. Some data is unable to be shared publicly. We detail how to get that below. The sections of this repo are: inputs, outputs, scripts.

Inputs contain data that are unchanged from their original. We use two datasets: 

- Democracy Fund + UCLA Nationscape survey results released on June 25th , 2020 is the individual survey level data used in the paper. 
Ciatation: Tausanovitch, Chris and Lynn Vavreck. 2020. Democracy Fund + UCLA Nationscape, October 10-17, 2019 (version 20200814). Retrieved from https://www.voterstudygroup.org/downloads?key=84a68f37-86ac-4871-b68a-a57b4d9e31d2.

- 2018 American Community Survey is the Post-stratification dataset used in the paper.
Citation: Steven Ruggles, Sarah Flood, Ronald Goeken, Josiah Grover, Erin Meyer, Jose Pacas and Matthew Sobek. IPUMS USA: Version 10.0 [dataset]. Minneapolis, MN: IPUMS, 2020.
https://doi.org/10.18128/D010.V10.0]

Outputs contain data that are modified from the input data, the report and supporting material.

- survey.csv, modified from the Democracy Fund + UCLA Nationscape project.
- cell_post.csv, modified from ACS data

Scripts contain R scripts that take inputs and outputs and produce outputs. These are:

- 01_data_cleaning.R
- 02_data_preparation.R
