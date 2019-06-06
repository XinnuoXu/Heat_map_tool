# heat map summarization

## Requirements <br />
* seaborn
* pandas
* numpy
* matplotlib

## HRED <br />

Preprocessing
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
