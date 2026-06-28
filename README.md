# Hardware-Trojan-Detection


 Final year Project for Research - 
Hardware Trojan Detection and Attribution Framework Using Multi-Modal Side-Channel Analysis, Formal Verification, and Machine Learning 


## Problem

Current hardware Trojan detection approaches suffer from:

* High false positives
* Difficulty detecting stealth Trojans
* Poor scalability
* Limited explain ability 

The research objective is to create a framework capable of:

1. Detecting Hardware Trojans
2. Classifying Trojan families
3. Identifying trigger mechanisms
4. Estimating attack severity
5. Producing explainable evidence


## Questions
Q1 - Can side-channel signals identify Hardware Trojans before activation?
Q2 - Can machine learning classify Trojan types?
Q3 - Can explainable AI identify malicious logic regions?
Q4 - Which side-channel feature contributes most to detection accuracy?


## Project becomes:

           Trojan Inserted
                  ↓
      Multi-Domain Measurements
                  ↓
          Feature Extraction
                  ↓
          ML Classification
                  ↓
        Explainability Engine
                  ↓
         Forensic Attribution
                 ↓
           Risk Assessment


## Research Architecture
                 ┌─────────────┐
                 │ FPGA Device │
                 └──────┬──────┘
                        │
      ┌─────────────────┼─────────────────┐
      │                 │                 │
      ▼                 ▼                 ▼

    Power Trace       Timing Trace         EM Trace

      │                 │                 │
      └────────────┬────┴────┬────────────┘
                   ▼

          Feature Extraction

                   ▼

      Machine Learning Engine

                   ▼

        Explainability Layer

                   ▼

          Forensic Dashboard

          
## Research Dataset Generation

## Designs - Develop multiple reference circuits like :

*  AES Encryption Core
* UART Controller
* Traffic Light Controller
* Memory Controller
* ALU Design
* RISC-V Processor Core


## Possible Open-Source Core:

### PicoRV32 
PicoRV32 is an excellent processor core for a Hardware Trojan Detection Homelab because it is a compact, open-source RISC-V CPU that is easy to understand, modify, simulate, and deploy on an FPGA. Its simplicity makes it ideal for experimenting with Trojan insertion and evaluating detection techniques without the complexity of a large commercial processor.


## Trojan Categories

Create several Trojan families.


### Type 1

 Information Leakage Trojan

      Secret Key
          ↓
    Hidden Register
          ↓
     Leak Channel

### Type 2

 Denial of Service Trojan

       Trigger
          ↓
     Infinite Loop
          ↓
      System Halt

###  Type 3

  Data Manipulation Trojan

        Input
          ↓
     Modify Output
          ↓
      Corrupt Data

### Type 4

  Time Bomb Trojan

      Counter
         ↓
    100000 Cycles
         ↓
     Activate     

### Type 5

Rare Trigger Trojan

      Trigger:
      1010110010110011

It's difficult to detect.

## Formal Verification Module

This project includes:

### RTL Equivalence Checking

Compare:

Golden RTL
vs
Trojan RTL

### Assertion-Based Verification

Example:

assert(output_data == expected_data);


### Model Checking

Verify:

* State transitions
* Trigger conditions
* Reachability

Research angle:

  Can formal verification discover hidden states?


## Side-Channel Acquisition

### Power Analysis

Measure:

Voltage
Current
Power

Sampling:

10 kHz
100 kHz
1 MHz


### Timing Analysis

Features:
* Critical path delay
* Slack
* Clock skew

  
### Switching Activity

Extract:

Toggle Rate
Transition Density

### Electromagnetic Analysis

Advanced track:
           Use inexpensive SDR.


Possible devices:
           * RTL-SDR
           * HackRF (if available)


Capture emissions from FPGA.


### Feature Engineering

Create feature vectors.

Example:

Mean Power

Peak Power

Variance

Standard Deviation

Skewness

Kurtosis

Entropy

Transition Count


## Machine Learning Layer

### Dataset

Trojan Present
Trojan Absent


## Models

*  Random Forest
*  XGBoost
*  Support Vector Machine
*  Isolation Forest
*  One-Class SVM
*  Autoencoder

  
## Deep Learning Extension

Use: 
   #### CNN
   
Input: 
   Power Trace Image

   #### LSTM   
   
Input:
   Time Series Signals


## Explainable AI

Use:
   #### SHAP
   #### LIME
   
Outputs:
     Feature Importance

     Most Suspicious Signal

     Detection Confidence


## Forensic Investigation Framework

Treat Hardware Trojan as a cybercrime scene.
 
Evidence Sources
FPGA Bitstream
Power Traces
EM Traces
Timing Reports
Waveforms
Logic Analyzer Data
Simulation Results


## Digital Evidence Management


      Evidence Collection
                ↓
             Hashing
                ↓
             Storage
                ↓
             Analysis
                ↓
            Reporting

            
Use:

#### SHA-256

Example:
        sha256sum trojan.bit

        
## Attribution Engine

Determine:

* Trojan Type
* Trigger Type
* Payload Type
* Severity

  
Example:

#### Attribute            Result

Family                    Data Leakage
Trigger                   Rare Input
Confidence                96.2%
Severity                  High


## Research Metrics

#### Detection Accuracy

      TP+TN
     -------
      Total

#### Precision

      TP
     -----
     TP+FP

#### Recall

      TP
     -----
     TP+FN
     
### F1 Score

#### Research target:  
Above 90%


### Experimental Design

##### Phase 1
Generate:  

50 Golden Designs

##### Phase 2

Insert:

100 Trojan Variants

##### Phase 3

Collect:

1000+ Traces

##### Phase 4

Train ML Models

##### Phase 5

Evaluate Detection


### Statistical Validation
 Use:    ANOVA
         T-Test
         Mann-Whitney U Test

Demonstrate significance.


### Dashboard Development

Create web dashboard.
Stack:
       * Python
       * Flask
       * SQLite
       * Plotly

       
Features:

   Live Detection

   Trojan Score
   
   Evidence Viewer

   Power Graphs

   Threat Alerts

    
### Dataset

1000+
Power Traces


#### Source Code

Verilog
Python
ML Models
Dashboard

#### Detection Framework

TrojanDetector.py

#### Forensic Toolkit

HardwareForensicsSuite












