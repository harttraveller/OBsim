# Description
OBsim: Outbreak simulation program

# Dependencies
- numpy
- plotly
- pandas
- python 3.7

# Tutorial

refer to tutorial.ipynb

# Parameters

#### starting_infected
- descr: number of individuals infected on day 1 of outbreak, suggested input is 1
- range: [ 0, inf ]

#### infected_growth_rate
- descr: daily percentage growth rate of infection, realistic inputs range from 0.01 to 0.1
- range: [ 0, inf  ]

#### awareness
- descr: starting awareness of virus, ranges from 0 to 1, increases based on multiplier so a 0 value will never increase
- range: [ 0, 1 ]

#### max_awareness
- descr: maximum internal awareness value - can not grow past this point
- range: [ 0, 1 ]

#### awareness_growth_rate
- descr: Daily percentage growth rate of awareness value
- range: [ 0, inf ]
  
#### mortality_day_rate
- descr: Daily percentage of infected that die
- range: [ 0, 1 ]
  
#### recovery_day_rate
- descr: daily percentage of infected that recover
- range: [ 0, 1 ]
  
#### recovery_multiplier
- descr: if people are known to be infected, they may recover faster, this represents a multiplier for the speed they recover if they are known to be infected
- range: [ 0, inf ]
  
#### containment_effectiveness
- descr:  what percentage of known infected patients are prevented from infecting others, if 0, containment is 0 percent effective, if 0.95, containment is 95% effective
- range: [ 0, 1 ]

#### cycles 
- descr: equivalent to number of days the simulation runs for
- range: [ 0, inf]



