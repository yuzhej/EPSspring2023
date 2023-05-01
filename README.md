# EPSspring2023
EPS Course Project Work

## Description

### Why this project is important?

There are growing interests in the Health industry to improve overall population health as the world’s population continues to grow and the increased travels promotes increased flow between countries.  One of great benefits from such focus is to prepare for any ongoing disease outbreaks, like COVID-19, by understanding these disease impacts and overcrowding. In order to focus on these disease related outbreaks, this project attempts to build predictive modeling for patient admissions. Overcrowding would happen when no ICU beds are available at the hospital to admit new patients, which could also be the result of admitting too many non-emergency patients.       

There are ways to build predictive modeling for incoming volume of patients utilizing overall population health but there are also some challenges, such as privacy. If privacy issues can be resolved, hospital operations and leadership will likely implement such a tool/product, which can save operational costs by appropriately allocating budgets for beds/work forces. 

### What this project does
In this project, I initially tested out TensorFlow Federated learning to understand the underlying algorithm for TensorFlow Federated learning by reading published papers and relevant working documentations and projects related to Federated learning. Once the fundamental understanding had been built, I installed TensorFlow Federated and started to run the demo guide on TensorFlow Federated learning. Then, I started to process COVID-19 datasets available on Centers for Disease Control and Prevention by exploring and cleaning data. 

### Background
I initially attempted to use the TensorFlow Federated framework (https://www.tensorflow.org/federated), developed and maintained by TensorFlow at Google (https://www.tensorflow.org), to work on this project. TensorFlow Federated (TFF) is a framework for building machine learning models that can be trained on decentralized data, such as data stored on user devices. TFF allows building, training, and testing machine learning models on data distributed across multiple data sources, like hospitals or users’ devices, without having to centralize the data, which enables privacy-preserving and scalable machine learning. TFF provides a set of tools for defining and executing federated computations, and for aggregating the results of these computations to update a global model. With such features, it can be utilized in real-world federated data to address the challenges of privacy. One example Google showed was Google Keyboard research on training models on individual devices and improving the shared model by sending only the model update.

### File Directory

There are three folders, Global, State, and charts, which include jupyter notebook files, underlying datasets and charts. 

#### global

Global folder includes "Federated Project Global.ipynb" file, which is the jupyter notebook file showing data processing of the entire COVID-19 case file and data models for the entire datasets to establish the global base model.

#### state

State folder includes "Federated State.ipynb" file, which is the jupyter notebook file showing data processing of the state level cases and date models for the local datasets to establish the local models. The folder also includes the inital local datasets - "table.csv" and "tabletranspose.csv"; and the result for the best model - "z.csv".

#### charts

charts folder includes png files showing graphs and charts derived from these jupyter notebook files. 
