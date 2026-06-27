# Hardware-Trojan-Detection


# Final year Project for Research -
Hardware Trojan Detection and Attribution Framework Using Multi-Modal Side-Channel Analysis, Formal Verification, and Machine Learning 


## Problem

Current hardware Trojan detection approaches suffer from:

High false positives
Difficulty detecting stealth Trojans
Poor scalability
Limited explain ability 

The research objective is to create a framework capable of:

Detecting Hardware Trojans
Classifying Trojan families
Identifying trigger mechanisms
Estimating attack severity
Producing explainable evidence


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

# Designs - Develop multiple reference circuits like :

# AES Encryption Core
# UART Controller
# Traffic Light Controller
# Memory Controller
# ALU Design
# RISC-V Processor Core


## Possible Open-Source Core:








