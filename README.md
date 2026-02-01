# ai-healthcare-coursework
Portfolio of AI and healthcare-related coursework, including Python-based simulation modelling, medical imaging (ultrasound), and data analysis projects. Prepared for research and internship applications.
# AI & Healthcare Coursework Portfolio

This repository contains selected coursework and projects from my **MSc Natural Sciences (Neuroscience, Psychology & Medical Physics)** degree at **University College London (UCL)**.  
It highlights my interests in **AI for healthcare**, **medical imaging**, and **computational modelling**, with a focus on clinically relevant applications.

---

# AI Healthcare Coursework – Virology Modelling Project

This repository contains a computational virology project developed as part of undergraduate coursework at University College London. The project implements a **cellular automata–based epidemic model** to simulate infectious disease spread and investigate the impact of quarantine and recovery dynamics on epidemic outcomes.

The work demonstrates skills in **Python-based modelling, experimental design, parameter sensitivity analysis, and interpretation of epidemiological data**, with a focus on healthcare-relevant applications.

---

## Project Overview

The model extends a classical SEIR framework into a **SEIQRH cellular automaton**, capturing spatial interactions between individuals and the effects of public health interventions such as quarantine and recovery support.

- **Framework:** Cellular automata epidemic model  
- **Grid size:** 6 × 6 (36 individuals)  
- **Neighbourhood:** Moore neighbourhood (8 adjacent cells)  
- **Time resolution:** 1 day per timestep  
- **Simulation length:** 60 days  

### Health States Modelled
- **S** – Susceptible  
- **E** – Exposed  
- **I** – Infected (symptomatic)  
- **Q** – Quarantined  
- **H** – Healing (self-recovery)  
- **R** – Recovered  

Each cell represents an individual whose state updates probabilistically based on neighbouring cells and epidemiologically informed transition parameters.

---

## Model Logic

At each timestep, every cell in the grid is updated according to its current state and the states of its immediate neighbours.

Key transition mechanisms include:
- **Infection:** Susceptible cells transition to Exposed based on contact with infected or healing neighbours
- **Disease progression:** Exposed cells transition to symptomatic infection after an incubation period
- **Intervention dynamics:** Infected individuals may enter quarantine or self-heal
- **Recovery:** Individuals recover either through quarantine-supported recovery or natural healing

The simulation tracks population-level trends by counting the number of individuals in each state at every timestep.

---

## Parameterisation

Model parameters were informed by epidemiological literature, including WHO reports and peer-reviewed studies.

Key parameters include:
- **SE:** Probability of infection after exposure  
- **EI:** Incubation transition probability (E → I)  
- **IQ:** Quarantine rate (I → Q), varied across cities  
- **HR:** Healing recovery rate (H → R)  
- **QR:** Quarantine recovery rate (Q → R), varied experimentally  

Quarantine rates were selected to reflect real-world differences (e.g. London, Wuhan, New York), while recovery rates were varied to assess healthcare resource impact.

---

## Experiments Conducted

Two main experimental analyses were performed:

### 1. Quarantine Recovery Rate (QR) Sensitivity
- QR values tested: **0.1, 0.2, 0.3**
- Other parameters held constant
- Objective: assess how post-quarantine care affects recovery speed and epidemic resolution

### 2. Quarantine Rate (IQ) Comparison
- IQ values reflecting different city-level responses
- Objective: evaluate the effect of isolation timing on transmission dynamics

For each parameter configuration:
- **100 independent simulation runs** were performed
- Results were averaged to ensure robustness and reduce stochastic noise

---

## Key Findings

- Higher quarantine recovery rates led to **earlier and faster population recovery**
- Increased QR reduced the **peak size and duration of symptomatic infection**
- Quarantine effectiveness significantly influenced epidemic duration and burden
- Model behaviour aligned with epidemiological expectations, supporting the validity of the chosen parameters

These results highlight the importance of recovery support and healthcare resources alongside isolation policies.

---

## Visual Outputs

The project includes:
- Time-series plots of Susceptible, Sick, and Recovered populations
- State-level breakdowns of infected subcategories (E, I, Q, H)
- Spatial visualisations showing disease progression across the grid

All figures were generated using **Python (NumPy, Matplotlib)**.

---

## Tools & Technologies

- **Programming language:** Python  
- **Libraries:** NumPy, Matplotlib  
- **Methods:** Simulation modelling, parameter sensitivity analysis, data visualisation  

---

## Learning Outcomes

This project strengthened skills in:
- Computational modelling of healthcare systems
- Translating biological assumptions into algorithmic rules
- Designing and analysing simulation experiments
- Interpreting results in a clinically and epidemiologically meaningful way
- Scientific communication through figures and structured reporting

---

## Notes

This repository is intended for **academic and portfolio demonstration purposes**. The model is simplified and does not represent real-world clinical predictions.

---

## Author

**Marya Cao**  
MSc Natural Sciences (Neuroscience, Psychology & Medical Physics)  
University College London  
