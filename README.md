# Code For Submitting Paper


## How to Run

1. Build conda env

```
pip install -r requirement.txt
```


2. Train

```shell
python train.py --config config/PEMS08/rmm_gwnet.py
```

the training log and other output files will be saved in 'save' dir.


## File Structure

```
- project
  - config
    - PEMS04
    - PEMS08
  - data
    - PEMS04
    - PEMS08
  - mtf
    - layers
    - models
    - utils
  - script
  - train.py
```

The datasets we use are from the standard PEMS04 and PEMs08 datasets. The pickle file of 'data' is a dictionary: 
```
{
  "timestamp": datetime()
  "flow": numpy(N, L),
  "speed": numpy(N, L),
}
```
