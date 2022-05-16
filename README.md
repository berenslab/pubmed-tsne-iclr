# Two-dimensional visualization of large document libraries using t-SNE
###### Rita González-Márquez, Philipp Berens & Dmitry Kobak

In this repository you can find the code associated to the paper "Two-dimensional visualization of large document libraries using t-SNE" (https://openreview.net/forum?id=Hebl3EZ16lq).

The notebooks 01-06 contain the code to reproduce all the analyes/experiments performed. The notebooks S1-S3 contain the experiments associated to the supplementary material. All figures included in the paper can be generated with these notebooks and will be stored in the `figures` folder.

In order to be able to run `01_dataset_preparation.ipynb`, the dataset needs to be first downloaded into the `data` directory from https://www.nlm.nih.gov/databases/download/pubmed_medline.html and then unziped. The data used in the paper was the 2020 baseline (not available anymore), but the 2021 baseline includes our data and new works published in 2021, plus revised, and deleted citations. For that the notebook `00_download_data.ipynb` can be used (it should be noted that the path to the pubmed baseline should be changed accordingly to which baseline you want to download).

As one runs the notebooks, the computed variables will be stored in the `variables` directory. In there, two subdirectories can be found: `all_data` for experiments with the whole dataset, and `subset_2M` for the UMAP comparison, and for the perplexity-based vs. uniform affinities comparison. These subdirectories also contain further subdirectories for each experiment performed with a different parameter set (exgg=1, 2, etc.) or a different method (UMAP, etc.).

As the dataset and the obtained variables are too large, they are not included in the repository. However, you can find the t-SNE embedding along with some metadate in here: (link).