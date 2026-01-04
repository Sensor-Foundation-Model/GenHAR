# GenHAR

## Dataset

We use SBHAR, MotionSense, Shoaib, and HHAR for evaluation. You could replace them with your own datasets.

## How to run

### (1) Training phase

```shell
python main_GenHAR.py --mode train -dataset SBHAR
```

For this command, we use uci dataset to train a model.

### (2) Testing phase (cross-dataset evaluation)

```shell
python main_GenHAR.py --mode cross_dataset -dataset SBHAR -target_dataset hhar
```

For this command, we use the model trained by SBHAR dataset to test on hhar dataset.
