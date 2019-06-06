# heat map summarization

This reposite create heat maps for each document in [XSUM](https://github.com/EdinburghNLP/XSum/blob/master/xsum-human-evaluation-data.tar.gz) dataset and its summary based on [Glove](https://github.com/maciejkula/glove-python) (Sorry, not BERT, since I haven't found a machine to ran the retrained BERT model). Each element in the heat map stands for the (1 - [cosine distance](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.spatial.distance.cosine.html)) between the term from document (x-axis) and the term from reference sumary (y-axis)

## Requirements <br />
* seaborn
* pandas
* numpy
* matplotlib

## Quick Start <br />

The cosine distances have been pre-calculated and stored in directory `csv_files`. The directories in `csv_files` is named as the document id. 

```
plot_doc('8004')
```
