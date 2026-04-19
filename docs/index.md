# Continuous Intelligence

This site provides documentation for this project.
Use the navigation to explore module-specific materials.

## How-To Guide

Many instructions are common to all our projects.

See
[⭐ **Workflow: Apply Example**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get these projects running on your machine.

## Project Documentation Pages (docs/)

- **Home** - this documentation landing page
- **Project Instructions** - instructions specific to this module
- **Glossary** - project terms and concepts

## Additional Resources

- [Suggested Datasets](https://denisecase.github.io/pro-analytics-02/reference/datasets/cintel/)

## Custom Project

### Dataset
I used `data/system_metrics_brandon.csv`, a system metrics dataset where each row represents one observation of system activity including requests, errors, and total latency.

### Signals
I used the original signals `error_rate` and `avg_latency_ms`, and I created a new signal called `successful_requests` calculated as requests minus errors.

### Experiments
I experimented by renaming the example files to my own Brandon versions, updating the input and output paths, and extending the pipeline logic by adding the `successful_requests` metric.

### Results
The modified pipeline ran successfully, detected anomalies based on the threshold rules, and produced an updated summary file in `artifacts/system_assessment_brandon.csv`.

### Interpretation
The results show how raw system data can be turned into useful monitoring insights, helping identify whether the system is stable or degraded and giving better operational awareness through the added successful requests metric.
