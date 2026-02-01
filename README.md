# ai-healthcare-coursework
Portfolio of AI and healthcare-related coursework, including Python-based simulation modelling, medical imaging (ultrasound), and data analysis projects. Prepared for research and internship applications.

# AI & Biomedical Coursework Portfolio  
**Marya Cao | UCL MSci Natural Sciences (Neuroscience, Psychology & Medical Physics)**

This repository contains selected academic coursework demonstrating my experience across **computational modelling**, **medical imaging**, and **biomedical research**, with applications relevant to **AI in healthcare**, **medical imaging**, and **data-driven analysis**.

The projects included highlight my ability to:
- Apply quantitative and computational methods to real-world biomedical problems  
- Analyse and interpret medical imaging data  
- Critically evaluate disease mechanisms with translational relevance  
- Communicate complex scientific concepts clearly and rigorously  

---

## 📊 Project 1: Computational Modelling of Viral Infection Dynamics (Virology)

### Overview  
This project implements a **Python-based cellular automaton epidemic model** to investigate viral transmission, quarantine, and recovery dynamics at a population level. A modified **SEIQ(H)R framework** was used to capture realistic infection pathways, including quarantine and self-healing states.

Each grid cell represents an individual, with probabilistic state transitions informed by epidemiological literature. The model simulates disease spread over discrete time steps and evaluates how public health interventions influence epidemic outcomes.

---

### Model Features  
- Discrete-time cellular automaton framework  
- Probabilistic state transitions based on literature-derived parameters  
- Explicit modelling of quarantine, recovery, and self-healing pathways  
- Spatial transmission via local neighbourhood interactions  
- Parameter sweeps and averaging across multiple simulation runs  

---

### Experimental Design  
- Simulated **60-day epidemic trajectories**  
- Performed **100 independent simulation runs per parameter set** to reduce stochastic noise  
- Investigated the impact of:
  - **Quarantine rate (IQ)**  
  - **Quarantine recovery rate (QR)**  
- Compared epidemic peaks, recovery timing, and infection duration across scenarios  

---

### Key Findings  
- Higher **QR values** resulted in earlier and more rapid recovery  
- Increased quarantine effectiveness reduced symptomatic peaks  
- The model reproduced realistic epidemic dynamics consistent with public health expectations  

---

### Skills Demonstrated  
- Python programming and simulation design  
- Data aggregation, visualisation, and performance evaluation  
- Parameter sensitivity analysis  
- Scientific reasoning and model validation  

---

## 📡 Project 2: Biomedical Ultrasound Imaging Coursework

### Overview  
This coursework explores the **physics and system-level controls of clinical diagnostic ultrasound imaging** through hands-on experiments using a clinical ultrasound machine. The focus was on understanding how acquisition parameters influence **image quality, resolution, penetration depth, and diagnostic interpretability**.

---

### Topics Investigated  

#### Time Gain Compensation (TGC)  
- Analysed depth-dependent attenuation and manual gain correction  
- Optimised near-field and far-field brightness for anatomical clarity  
- Evaluated diagnostic consequences of incorrect TGC settings  

#### Dynamic Range  
- Compared images acquired at 50 dB, 70 dB, and 90 dB  
- Assessed contrast versus soft tissue detail trade-offs  
- Demonstrated loss of subtle features at low dynamic ranges  

#### Frequency & Harmonic Imaging  
- Compared imaging at 6.6 MHz, 10 MHz, 14 MHz, and harmonic modes  
- Evaluated resolution–penetration trade-offs  
- Observed improved contrast and reduced artefacts in harmonic imaging  

#### Transmit Focusing & Frame Rate  
- Investigated multi-transmit focusing and focal depth alignment  
- Analysed frame rate reduction with increased focal zones  
- Demonstrated how focal depth controls lateral resolution  

#### Spatial Resolution Analysis  
- Measured axial and lateral resolution using wire phantoms  
- Applied diffraction theory to explain depth-dependent resolution loss  

---

### Skills Demonstrated  
- Clinical ultrasound system operation  
- Medical image interpretation and optimisation  
- Quantitative resolution analysis  
- Linking physical imaging principles to clinical outcomes  

---

### Relevance to AI & Medical Imaging  
This coursework provides a strong foundation for:
- Medical image preprocessing  
- AI-based segmentation and classification  
- Understanding artefacts and limitations in real-world ultrasound datasets  

---

## 🧠 Project 3: Literature Review — Neuroinflammation and Tau Pathology in Alzheimer’s Disease

### Overview  
This literature review examines **tau protein dysregulation** as a central mechanism in Alzheimer’s disease, with a focus on phosphorylation-driven misfolding and aggregation processes relevant to neurodegeneration.

---

### Key Mechanistic Insights  

Under physiological conditions, tau is a highly soluble, intrinsically disordered microtubule-associated protein that stabilises axonal microtubules. Its conformational flexibility is tightly regulated by a balance between phosphorylation and dephosphorylation, mediated primarily by kinases such as **GSK3β** and **CDK5**, and the phosphatase **PP2A**.

Disruption of this equilibrium represents a critical early event in Alzheimer’s disease. Aberrant phosphorylation at multiple serine, threonine, and tyrosine residues reduces tau’s affinity for microtubules, promoting its detachment into the cytosol and increasing conformational instability.

As tau becomes increasingly hyperphosphorylated, it adopts aggregation-prone conformations that favour self-association, leading to the formation of early misfolded intermediates. These intermediates act as **seeding-competent species**, capable of templating the misfolding of native tau in a prion-like manner. This seed formation represents the **rate-limiting step** in tau aggregation and establishes the foundation for downstream pathological amplification.

---

### Skills Demonstrated  
- Critical evaluation of biomedical literature  
- Mechanistic reasoning in neurodegenerative disease  
- Translational thinking linking molecular pathology to therapeutic relevance  
- Clear scientific writing and synthesis  

---

## 🔬 Overall Skill Set Highlighted  
- Python-based modelling and data analysis  
- Medical imaging fundamentals (ultrasound)  
- Experimental design and parameter analysis  
- Biomedical literature synthesis  
- Interdisciplinary AI–healthcare research foundations  

---

## 📌 Future Directions  
- Extending epidemic models with real-world datasets  
- Applying deep learning methods to ultrasound image segmentation  
- Integrating physics-based understanding into AI medical imaging pipelines  
