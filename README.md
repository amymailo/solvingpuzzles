# solvingpuzzles


## Summary 
In this puzzle project, we explore a solution for jigsaw puzzles, inspired by a scholarly paper titled "A fully automated greedy square jigsaw puzzle solver" (CVPR 2011, D. Pomeranz et al.). The paper introduces a method to solve square jigsaw puzzles without prior knowledge of the image or its parts' locations.

Our project adapts the idea using a neural network with a U-Net-like architecture to predict how puzzle pieces should be arranged. We evaluate the model's performance subjectively by visualizing predicted arrangements and objectively by calculating accuracy on a test set.

To test the reproducibility of our code, we create a new dataset. Our approach is inspired by the scholarly work's emphasis on compatibility metrics for predicting piece adjacency.

D. Pomeranz, M. Shemesh and O. Ben-Shahar, "A fully automated greedy square jigsaw puzzle solver," CVPR 2011, Colorado Springs, CO, USA, 2011, pp. 9-16, doi: 10.1109/CVPR.2011.5995331.



# Overview
In this puzzle project, we explore an existing solution for solving jigsaw puzzles, accessible at this Kaggle link (https://www.kaggle.com/datasets/serhiibiruk/jigsaw-puzzle). The provided code employs a neural network-based approach utilizing a U-Net-like architecture to predict the permutation of pieces in a puzzle.


## Key Features Model Architecture

The code implements a U-Net-like neural network to predict the arrangement of jigsaw puzzle pieces.
The model is trained to reconstruct the correct arrangement from shuffled inputs.
Performance Evaluation:

The effectiveness of the model depends on data quality, model architecture, and hyperparameters.
Evaluation is conducted on a test set, and accuracy is calculated based on reshaped ground truth labels and predicted labels.


## Considerations

### Failure Cases:

The model may encounter failure cases where it struggles to accurately predict the arrangement of puzzle pieces, particularly in complex or ambiguous scenarios.

### Evaluation Methods:

- Subjective: Visualization of predicted arrangements using the provided rearrange function.
- Objective: Quantitative evaluation using accuracy metrics on a test set.


## Reproducibility
We aim to test the reproducibility of the provided code by implementing similar code and creating a new dataset. This approach ensures a robust assessment of the model's performance and generalizability to different puzzle configurations. Here is the dataset we created ([https://www.kaggle.com/datasets/68c01d9e96297772024708405f92f941fb1bfc919ae9f4a9df52ed889f1f2640](https://kaggle.com/datasets/bbec2171f34965a432783efb7b709e6a7ff5a3e8cde6b2fe5060fe29bb6d111f
)). Within this respository, you can find the code we used. 


## Next Steps
If you are interested in experimenting with the code, we recommend:
- Customizing the model architecture based on your specific puzzle characteristics.
Exploring alternative loss functions or metrics for better alignment with your objectives.
Documenting and sharing details of your experimentation process for transparency and reproducibility.
Feel free to adapt and build upon this code to suit your puzzle-solving needs.
