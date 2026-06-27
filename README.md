# Hardware-Trojan-Detection




Research Problem
Current hardware Trojan detection approaches suffer from:
High false positives
Difficulty detecting stealth Trojans
Poor scalability
Limited explainability
The research objective is to create a framework capable of:
Detecting Hardware Trojans
Classifying Trojan families
Identifying trigger mechanisms
Estimating attack severity
Producing explainable evidence
Research Questions
RQ1
Can side-channel signals identify Hardware Trojans before activation?
RQ2
Can machine learning classify Trojan types?
RQ3
Can explainable AI identify malicious logic regions?
RQ4
Which side-channel feature contributes most to detection accuracy?
Novel Contribution
Most student projects stop at:
Trojan Inserted
↓
Power Increased
↓
Detected
Your project becomes:
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
Research Architecture
                 ┌─────────────┐
                 │ FPGA Device │
                 └──────┬──────┘
                        │
      ┌─────────────────┼─────────────────┐
      │                 │                 │
      ▼                 ▼                 ▼

 Power Trace      Timing Trace     EM Trace

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
Research Dataset Generation
Golden Designs
Develop multiple reference circuits:
AES Encryption Core
UART Controller
Traffic Light Controller
Memory Controller
ALU Design
RISC-V Processor Core
Possible open-source core:
