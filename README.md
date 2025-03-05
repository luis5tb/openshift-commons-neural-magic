# OpenShift Commons Neural Magic Workshop

This repository contains workshop materials and examples for creating optimized models with Neural Magic solutions on OpenShift. The workshop is part of the OpenShift Commons initiative.

## Overview

This workshop demonstrates how to leverage Neural Magic's model optimization techniques (`llm-compressor`) on OpenShift. Learn how to achieve significant performance improvements and cost reductions through model sparsification and quantization.

## Repository Structure

### Workbenches

The `workbenches/` directory contains Jupyter notebooks and interactive environments for:
- Model optimization techniquies:
  - Weights quantization: `int4`
  - Weights and activations quantization: `fp8` and `int8`
- Model accuracy/performance evaluation

### Pipelines

The `pipelines/` directory includes automated workflows for:
- Model quantization pipelines for optimizing models while maintaining accuracy
- Also includes evaluation steps
- Readme with instructions to create and run the pipeline

## Getting Started

### Prerequisites

- OpenShift AI
- NVIDIA GPUs

### Usage

1. Go to Data Science Projects in OpenShift AI and create a new project.
2. Ensure a pipeline server is configured.
3. Create a workbench in the project.
   a) Select Standard Data Science.
   b) Select medium size and add a GPU to it.
4. Clone this repository: https://github.com/your-org/openshift-commons-neural-magic.git.
5. Go to the workbenches folder and follow the setup instructions in each workbench.
6. Once done with the workbenches, go to the pipeline folder and compile the pipeline. Follow instructions in the README.md file at the pipeline folder.
7. Download the created pipeline yaml file and import it in OpenShift AI, Data Science Pipelines.
8. Run the pipeline.
