#  Non-exhaustive taxonomy of efficiency metrics

> *"To deploy a model, typically we can measure its feasibility via its performance (quality metrics like accuracy, precision, and recall) and cost (footprint metrics like model size, latency, and number of epochs to convergence). To compare any two given models for their relative efficiency, it is essential to compare both quality and footprint metrics."* [DOI:10.1145/3578938](https://dl.acm.org/doi/10.1145/3578938)

```mermaid
---
title: "Non-exhaustive taxonomy of efficiency metrics."
---
flowchart TD
    Efficient["`Efficient Metrics`"] --> Quality["`Quality Metrics`"]
    Efficient --> Footprint["Footprint Metrics"]
    Quality --> 
    QualityExamples["Accuracy

     Precision

     Recall

     AUC

     F1"] 
    Footprint --> TrainingInf["Training & Inference"] 
    Footprint --> TrainingOnly["Training Only"]
    Footprint --> InferenceOnly["Inference Only"]
    TrainingInf --> 
    FLOPSetc["Number of FLOPS

    Number of Parameters

    RAM consumption (peak,avg)"]
    TrainingOnly -->
    Epoch["Number of Epochs to converge

    Model Latency (backward pass)

    Number of labels required"]
    InferenceOnly --> Model["Model disk size
    
    Model latency (forward pass)"]
```