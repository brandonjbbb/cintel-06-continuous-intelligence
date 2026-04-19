# cintel-06-continuous-intelligence

[![Docs](https://img.shields.io/badge/docs-GitHub%20Pages-blue)](https://denisecase.github.io/cintel-06-continuous-intelligence/)
[![CI Status](https://github.com/denisecase/cintel-06-continuous-intelligence/actions/workflows/ci-python-zensical.yml/badge.svg?branch=main)](https://github.com/denisecase/cintel-06-continuous-intelligence/actions/workflows/ci-python-zensical.yml)
[![Python 3.14+](https://img.shields.io/badge/python-3.14%2B-blue?logo=python)](#)
[![MIT](https://img.shields.io/badge/license-see%20LICENSE-yellow.svg)](./LICENSE)

> Professional Python project for continuous intelligence.

Continuous intelligence systems monitor data streams, detect change, and respond in real time.
This course builds those capabilities through working projects.

In the age of generative AI, durable skills are grounded in real work:
setting up a professional environment,
reading and running code,
understanding the logic,
and pushing work to a shared repository.
Each project follows the structure of professional Python projects.
We learn by doing.

## This Project

This project brings together several techniques used in continuous intelligence systems.

The goal is to copy this repository,
set up your environment,
run the example analysis,
and explore how monitoring techniques can be combined
to assess the current state of a system.

Run the example pipeline, read the code, and see how:

- raw system metrics are transformed into useful signals
- anomalies are detected in those signals
- monitoring results are summarized to assess system health

This project demonstrates how monitoring data can support operational awareness and decision-making.

This module serves as a capstone:
it encourages you to combine techniques developed
in earlier modules into a simple continuous intelligence pipeline:

- Module 2. anomaly detection
- Module 3. signal design
- Module 4. rolling monitoring
- Module 5. drift comparison
- Module 6. system assessment (integration)

## My Modification

I modified the project by creating my own Brandon versions of the example files and updating the pipeline to use my renamed dataset and Python module.

I changed the input file to `data/system_metrics_brandon.csv`, changed the output file to `artifacts/system_assessment_brandon.csv`, and renamed the source file to `src/cintel/continuous_intelligence_brandon.py`.

I also added a new derived metric called `successful_requests`, which is calculated as requests minus errors.

I made this change to better understand how small modifications to a continuous intelligence pipeline affect the logic, summary output, and final assessment.

After running the modified project, I observed that the pipeline executed successfully, created the artifacts folder when needed, and produced an updated summary file with my additional metric.

## Data

The modified pipeline reads system metrics from:

`data/system_metrics_brandon.csv`

Each row represents one observation of system activity.

The pipeline derives signals such as:

- **error_rate**
- **avg_latency_ms**
- **successful_requests**

It checks for anomalous conditions and produces a summary assessment of system behavior.

The dataset includes a short period of degraded performance so that monitoring signals and anomaly detection produce visible results.

## Output

The modified pipeline writes its final summary to:

`artifacts/system_assessment_brandon.csv`

This output file includes summary metrics for the system and a final `system_state` label showing whether the system is assessed as `STABLE` or `DEGRADED`.

## Working Files

You'll work with just these areas:

- **data/** - input data files
- **docs/** - project documentation
- **src/cintel/** - source code for the pipeline
- **artifacts/** - generated output files
- **pyproject.toml** - authorship and project configuration
- **zensical.toml** - authorship and project links

## Instructions

Follow the workflow guide to complete:

1. Phase 1. **Start & Run**
2. Phase 2. **Change Authorship**
3. Phase 3. **Read & Understand**
4. Phase 4. **Modify**
5. Phase 5. **Apply**

## Challenges

Challenges are expected.
Sometimes instructions may not exactly match your operating system or environment.
When issues occur, share screenshots, error messages, and details about what you tried.
Working through issues is part of implementing professional projects.

## Success

After completing the setup and modification steps, the project should run successfully and print:

```shell
========================
Pipeline executed successfully!
========================
