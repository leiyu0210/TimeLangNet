# TimeLangNet on UEA Dataset


## Install Requirements
**Step 1**: To get started with this repository, you'll need to follow these installation steps. Before proceeding, make sure you have [Pytorch](https://pytorch.org/get-started/previous-versions/) installed. 
```
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

**Step 2**: Then install the rest of the required packages:
```
cd langnet
pip install -r requirements.txt
```

**Step 3**: Finally, install the `jupyter notebook` package:
```
pip install jupyter notebook
```


## Data Selection

You can test different datasets by changing the 'dataset_names' in the following code:

```
path="Multivariate_ts/" #datasets path 
flist = pd.read_csv("MSTC_Data.csv", header=None)
flist = flist.to_numpy().tolist()

print(flist)

def readucr(filename):
    data= load_from_tsfile_to_dataframe(filename)
    return data
dataset_names = [['Dataset Name']]
```






