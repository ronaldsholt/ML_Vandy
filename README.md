readme proj file

# ML Project - VAE for Pattern Rec.

Background:
- Predicting cell lineage patterns in RNAseq measurments.

Project Description: 
- Using representation learning as low dimentional input to higher dimentional reduction clustering tools like TSNE or UMAP to learn cell lineage. Also evaluate against traditional methods like PCA or Logistic PCA.

- Steps in the process:
1. Build encoder, decoder networks.
2. Train model on individual cell type RNAseq data.
3. Minimize objectively for MSE where train_data = {train_, train_}
4. Encoder instantiated seperatedly for classification
5. Use encoded RNAseq data to classify cell types
6. Use embedded latent vectors as input to TSNE/UMAP for further trajectory analysis

Performance Metric:
- Reconstruction Error: Min{L2-norm/MSE}
- Encoder classification: Confusion Maxtrix: Accuracy Report

## Description of Metrics:

### MSE:
1. Mean Squared Error: This measures the average sqaured distance, or errors, in the estimated value predictions and the ground truth values. In our problem, we generte a reconstructed version of our input to the network.  We aim to minimze this distnce, or reconstruction error, to check the ability of our network to learn the parameters of our data. 


### Confustion Matrix
Confusion Matrix - Multi-Classification
Positive = Uqniue Cell Type
Negative = Mixed Cell Type

- True Positive
  - We predict an cell as a cell in a trajectory and it is that cell type in that trajectory 
- False Positive
  - We predict an cell is a type that is not in a trajectory that is its true traj. 
  - In research, particularly targeted medicine, we would target wrong cell.
- False Negative

- True Negative
 
