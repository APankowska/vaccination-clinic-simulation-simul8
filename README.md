# vaccination-clinic-simulation-simul8
Discrete-event simulation of a COVID-19 vaccination clinic built in Simul8. The project models patient flow, queue dynamics, and staffing scenarios to identify bottlenecks, reduce waiting times, and optimise operational costs. Includes comparative analysis of two models to support data-driven healthcare decision-making.


# Vaccination Clinic Simulation – Management Science Project

## Project Overview
This project presents a discrete-event simulation model of a COVID-19 vaccination clinic developed in Simul8.

The objective was to: 
 - maximise the number of vaccinated patients,
 - minimise staff costs,
 - reduce waiting times,
 - identify process bottlenecks,
 - support data-driven managerial decisions.
   
The clinic operates 11 hours per day with varying arrival rates and limited staffing resources.

## Model Description
### Process Flow
Patients go through the following stages:
 - Registration
 - Health check
 - Vaccination
 - Observation / refreshment area
   
### Two scenarios (models) were developed:
 - Model 1 – baseline staffing configuration
 - Model 2 – reduced staffing with optimised resource allocation

## Input Data
#### Patient Arrival Distribution (Exponential)
| Time of Day | Arrivals per hour |
|-------------|-------------------|
| 8–9am | 12 |
| 9–11am | 6 |
| 11am–1pm | 12 |
| 1–4pm | 6 |
| 4–6pm | 15 |
| 6–7pm | 0 |

#### Process Time Distributions
| Process | Distribution | Parameters|
|---------|--------------|-----------|
| Registration | Triangular | 0.5, 1.5, 1 |
| Health Check | Triangular | 8, 25, 15 |
| Vaccination | Triangular | 5, 15, 9 |
| Refreshments | Fixed | 15 |

## Results
### Model 1 (Baseline)
 - 80 people vaccinated
 - Daily savings: £9,600
 - Staff cost: £8,907.72
 - Overall profit: £692.28
### Model 2 (Optimised Resources)
 - 74 people vaccinated
 - Savings: £8,880
 - Staff cost: £1,615.32
 - Overall profit: £7,264.68

## Key Findings
 - Reducing staff significantly lowers operational costs.
 - Smaller queue capacities reduce waiting times.
 - Model 2 generates higher financial profit.
   
However, Model 1 vaccinates more patients, which may be preferable from a public health perspective.


## Recommendation
 - If the objective is financial efficiency, Model 2 is optimal.
 - If the objective is maximising public health impact, Model 1 is preferable due to higher vaccination throughput.
   
This project demonstrates how simulation modelling can support strategic healthcare decision-making.

## Tools Used
#### Simul8
 - Process modelling
 - Queue analysis
 - Bottleneck identification
 - Cost-benefit analysis
