## ENCODE bigWig Analysis

This notebook provides an exploratory data analysis (EDA) of bigWig files from the ENCODE project, focusing on chromosome 10 at a 10kb resolution. Below is a summary of the key steps and analyses performed:

### Library Imports
- Imported essential libraries such as `pandas`, `numpy`, `sklearn.decomposition`, `matplotlib.pyplot`, and `seaborn`.
- Imported helper functions from `hwutils.py`.

### Data Loading
- Loaded a DataFrame of bigWig data binned to 10kb resolution across chromosome 10.
- Loaded metadata for the bigWig files.

### Data Visualization
- Visualized signal profiles on chromosome 10, focusing on dips around 40Mb.
- Created line plots using Seaborn to display data trends and patterns.

### Principal Component Analysis (PCA)
- Performed PCA to reduce dimensionality and visualize data.
- Compared different PCA methods, including standard PCA and PCA using Multidimensional Scaling (MDS).
- Normalized the data before performing PCA.

### Discussion on PCA and NMF
- Discussed the differences between PCA and MDS PCA.
- Explored the suitability of Non-negative Matrix Factorization (NMF) for the dataset, highlighting its advantages in representing gene expression data.

## Key Findings
- Identified significant dips in signals on chromosome 10 around 40Mb.
- Observed differences between standard PCA and MDS PCA, with MDS PCA showing a large cluster in the bottom left of the plot.
- Concluded that NMF would be useful for this dataset due to its non-negative representation of gene expression data.

This summary encapsulates the major components and findings of the analysis. For detailed code and results, please refer to the specific cells in the notebook.
