# reproducible-research-IA369Z

# A predictive DASH QoE approach based on machine learning at Multi-Access Edge Computing 
# Abstract
Network operators expected to run on with fast-growing multimedia video streaming (e.g., DASH) traffic demand while providing a high Quality of Experience (QoE) to the end-users. The cost, complexity, and scalability of existing QoE estimation solutions have significant limitations to infer QoE from network traffic. However, this works provides an end-user QoE estimation method based on a predictive passive QoE probe mechanism of DASH mobile video using a Machine Learning (ML) approach running at network edge nodes. We describe the design and implementation of probe configuration at the target edge, with traffic flow monitoring to generate network-level Quality of Service (QoS) metrics. Moreover, build a QoS-QoE correlation ML model in realtime fashion for detecting patterns of the user equipment traffic behavior to predict user QoE.

## Workflow
![alt text](https://github.com/sajibtariq/reproducible-research-IA369Z/blob/master/figures/Project%20workflow.jpg?raw=true)

## Requirements
**Data Aquisition**

[Testbed](https://github.com/sajibtariq/reproducible-research-IA369Z/tree/master/testbed)

**Data Pre-processing, Data Analysis & Executable Paper**

[Jupyter Notebook followed by Anaconda](https://docs.anaconda.com/anaconda/install/)
```bash
- Numpy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
```

[Scappy](https://anaconda.org/conda-forge/scapy)

[Imbalanced-learn- python package](https://anaconda.org/conda-forge/imbalanced-learn)

## Folder Stucture Scheme
* /data : Exported CSV file during preprocess from raw data
* /deliver : Executable notebook 
* /dev : Notebook along with data pre-process and analysis codes
* /figures : Research realted figures
* /testbed : Data generation testbed aligned with codes
* /tesbed/experiment : Raw network data & video log strorage
## Execute the Work
**Option 1:** Fully Exucute in local Machine - Ubuntu 18.04

**Note:** Testbed setup, data generation and raw data pre-process steps requires a lot time ans storage to finish. If you want you could sskip this option and follow the Opetion 2 or Option3

```bash
Envirionment Setup
```
Step 1: [Testbed Setup](https://github.com/sajibtariq/reproducible-research-IA369Z/tree/master/testbed)

Step 2: [Jupyter Notebook followed by Anaconda](https://docs.anaconda.com/anaconda/install/)

Step 3: [Scappy](https://anaconda.org/conda-forge/scapy)

Step 4: [Imbalanced-learn- python package](https://anaconda.org/conda-forge/imbalanced-learn)

```bash
Data Generation
```
Step 1: Open terminal and execute the following command

$ cd ~/reproducible-research-IA369Z/testbed/

$ sudo python3 test_1.py

```bash
Data Preprocess 
```
Step 1: Open jupyter notebook and open the **execute-draft.ipynbfile** from **~/reproducible-research-IA369Z/deliver/** directory

Raw data to export csv:

Step 2:  Run the cell that contains  **%run ./Raw-data-preprocess-&-csv-export.ipynb** this line 

Split training and testing CSV from exported csv:

Step 3:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/preprocess.ipynb** this line 


**Option 2:** Fully Exucute by provided pre-built VM images including all setup.

The VM images are in .ova format and should be usable with any modern x64 virtualization system.

[52 GB Size] - Ubuntu 18.04 x64 - Dash (pass: dash)

**Note:** If you are able to download the  VM image and import successfully but later not able to perform data generation and raw data preprocess steps inside VM properly due to any technical problem then just skip the Data Generation and Data Preprocess(Raw data to export csv) steps. You can still partially excute the work by completing  only  Data Preprocess(Split training and testing CSV from exported csv) and Data analysis steps with given dataset in  **~/reproducible-research-IA369Z/data/** directory

```bash
Data Generation
```
Step 1: Open terminal and execute the following command

$ cd ~/reproducible-research-IA369Z/testbed/

$ sudo python3 test_1.py

```bash
Data Preprocess 
```
Step 1: Open jupyter notebook and open the **execute-draft.ipynbfile** from **~/reproducible-research-IA369Z/deliver/** directory

Raw data to export csv:

Step 2:  Run the cell that contains  **%run ./Raw-data-preprocess-&-csv-export.ipynb** this line 

Split training and testing CSV from exported csv:

Step 3:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/preprocess.ipynb** this line 


```bash
Data Analysis
```
Step 1:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/model_accuracy_with_grid_search.ipynb** this line

Step 2:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/rfc.ipynb** this line



**Option 3:** Partially exucute if not able to perfom Option 1/2 or want to skip Opetion 1/2 (more spceficallly skip testbed setup, data generation and raw data preprocess steps)

```bash
Envirionment Setup- I woudl suggest use ubuntu 18.04
```
Step 1: [Jupyter Notebook followed by Anaconda](https://docs.anaconda.com/anaconda/install/)

Step 2: [Scappy](https://anaconda.org/conda-forge/scapy)

Step 3: [Imbalanced-learn- python package](https://anaconda.org/conda-forge/imbalanced-learn)

```bash
Clone git repository 
```
Step 1: Open terminal and execute the following command

$ git clone https://github.com/sajibtariq/reproducible-research-IA369Z.git


```bash
Data Preprocess 
```
Step 1: Open jupyter notebook and open the **execute-draft.ipynbfile** from **~/reproducible-research-IA369Z/deliver/** directory

Split training and testing CSV from exported csv:

Step 2:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/preprocess.ipynb** this line 


```bash
Data Analysis
```
Step 1:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/model_accuracy_with_grid_search.ipynb** this line

Step 2:  Run the cell that contains  **%run ~/reproducible-research-IA369Z/dev/rfc.ipynb** this line



## Distrubution
```bash
TODO
```
