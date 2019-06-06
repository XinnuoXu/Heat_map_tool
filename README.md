# heat map summarization

This reposite create heat maps for each document in [XSUM](https://github.com/EdinburghNLP/XSum/blob/master/xsum-human-evaluation-data.tar.gz) dataset and its summary based on [Glove](https://github.com/maciejkula/glove-python) (Sorry, not BERT, since I haven't found a machine to ran the retrained BERT model). Each element in the heat map stands for the (1 - [cosine distance](https://docs.scipy.org/doc/scipy-0.14.0/reference/generated/scipy.spatial.distance.cosine.html)) between the term from document (x-axis) and the term from reference sumary (y-axis)

## Requirements <br />
* seaborn
* pandas
* numpy
* matplotlib

## Quick Start <br />

The cosine distances have been pre-calculated and stored in directory `csv_files`. The directories in `csv_files` is named as the document id. Run `ipython notebook` and open `heat_map.ipynb`. Replace the `8004` in the following line with the document id you are interested in. 

```
plot_doc('8004')
```

Run all cells in the `heat_map.ipynb`. The heat maps of each document sentence and reference summary will appear. 

![alt text](https://github.com/XinnuoXu/heat_map_summarization/blob/master/show_case.png)
