readme proj file

# ML Project - VAE for Pattern Rec.

Background:
- Predicting cell lineage patterns in RNAseq measurments.

Project Description: 
- Using representation learning as low dimentional input to higher dimentional reduction clustering tools like TSNE or UMAP to learn cell lineage. Also evaluate against traditional methods like PCA or Logistic PCA.

Performance Metric:
- Min{L2-norm/MSE}

## Description of Metrics:

### MSE:
1. Mean Squared Error: This measures the average sqaured distance, or errors, in the estimated value predictions and the ground truth values. In our problem, we generte a reconstructed version of our input to the network.  We aim to minimze this distnce, or reconstruction error, to check the ability of our network to learn the parameters of our data. 
