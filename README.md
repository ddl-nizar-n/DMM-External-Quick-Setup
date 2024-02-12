# DMM-Quick-Setup

Setup scripts to create a Domino Model Monitoring demo model.

<p align="center">
<img src = https://github.com/ddl-dave-heinicke/DMM-Quick-Setup/blob/main/readme_images/Iris_Overview.png width="800">
</p>


## Background

These examples help create starter models in Domino Model Monitoring (DMM). 

Model monitoring can monitor Domino Model APIs (called Integrated Model Monitoring) or external models.
External models include models run as batch jobs without a model API and models hosted outside of Domino.

## Integrated Model Monitoring Example (Using a Domino Model API)

To get started, begin with one of the Integrated_DMM_Quickstart notebooks.

The high level steps are:

### I. Train Your Model

(1) Train a model and reister it in Domino's Model Catalog. Be sure that this model invokes Domino's DataCaptureClient so that Domino can automatically capture inference data.

(2) Register the data used to train that modlel as a Training Dataset. This is our baseline for data drift detection.

(3) Spin up a Domino Model API from the registered model.

(4) Once your model is running, register your model with Domino Model Monitoring.

### II. Capture Data Drift

(5) Send some test data to your model, to begin configuring drift detection.

(6) Wait until the initial inference data has ingested. This taks about an hour the first time.

(7) Schedule drift data checks.

### III. Capture ground truth labels for Model Quality monitoring




