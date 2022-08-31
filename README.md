# Pyramidal-Attention-Mechanism-For-Synthetic-Battery-Data-Generation

## Get started
This project has been executed via google colab.

#### Steps To Follow:

1. Download the code from github as a zip file.

2. Extract the contents of the zip file and upload it into google drive.

3. The code to be executed in google colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vageeshmaiya/Pyramidal-Attention-Mechanism-For-Synthetic-Battery-Data-Generation-/blob/main/Pyramidal_Attention_Mechanism_For_Synthetic_Battery_Data_Generation.ipynb)

4. Make sure to set the runtime to GPU before running the code.

5. Make the necessary changes mentioned in the code to get the result.

6. The dataset to be used has to be uploaded in the `data/datasets/` folder(if not already present).

## Usage:

To train and evaluate Pyraformer on a dataset the following command is used in the google colab notebook :

```train & evaluate
!python -u long_range_main.py -data Battery -data_path new_data.csv -input_size 100 -predict_step 24 -n_head 6 -run_name new_data_trial_1_24
```
The detailed descriptions about the arguments are as following:

| Parameter name | Description of parameter |
| --- | --- |
| data | The dataset name |
| data_path | The name of the csv file to be used |
| predict_step | The prediction horizon |
| run_name | The folder name used to save the output. This can be set to any word |


After running the main code , the output can be found in `results/run_name/` folder.

Any other changes such as `epoch` or `batch_size` can be done in the `long_range_main.py` script.

## Acknowledgement:

We appreciate the following github repos a lot for their valuable code base and datasets:

https://github.com/alipay/Pyraformer

Diao, W., Saxena, S., Pecht, M. Accelerated Cycle Life Testing and Capacity Degradation Modeling of LiCoO2 -graphite
 Cells. J. Power Sources 2019, 435, 226830
 
 Calce Battery Research Group. [Online]. Available: https://web.
calce.umd.edu/batteries/data.htm

