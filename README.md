# heat map summarization

This reposite create heat map for each document in [XSUM](https://github.com/EdinburghNLP/XSum/blob/master/xsum-human-evaluation-data.tar.gz) dataset and its summary based on [Glove](https://github.com/maciejkula/glove-python) (Sorry, not BERT, since I haven't found a machine to ran the retrained BERT model). Each element in the heat map stands for the (1 - [cosine distance](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.spatial.distance.cosine.html)) between the term from document (x-axis) and the term from reference sumary (y-axis)

## Requirements <br />
* seaborn
* pandas
* numpy
* matplotlib

## Quick Start <br />


```
sh preprocess_s2s.sh
```
Training

```
sh train_seq_lstm_2_seq.sh
```

Testing
```
sh predict_s2s.sh
```

## Graph to Sequence <br />
Preprocessing
```
sh preprocess_g2s.sh
```
Training

```
sh train_srl_seq-gcn_2_seq.sh
```
or for self-attn

```
sh train_srl_seq-gcn-selfattn_2_seq.sh
```

Testing
```
sh predict_g2s.sh
```

## Graph to TrDec <br />
Preprocessing
```
sh preprocess_g2g.sh
```
Training

```
sh train_srl_srl-gcn-selfattn_2_seq.sh
```

Testing
```
sh predict_g2g.sh
```
