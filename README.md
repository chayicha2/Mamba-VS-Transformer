# Model Comparison: Mamba vs Transformer

In this project, we implemented and compared the **Mamba** and **Transformer** models using the **same dataset** and **same number of epochs** (5 epochs) to solve a sequence-to-sequence regression task. The comparison aimed to evaluate model performance under identical conditions, with a focus on training efficiency and model complexity.

Both models were able to solve the same problem and achieve similar accuracy. However, there were significant differences in terms of **parameter count** and **training time**, which are detailed below.

### Key Findings
- **Dataset and Task**: Both models were trained on the same synthetic dataset to predict output values based on input features, ensuring a fair comparison.
- **Training Epochs**: Both models underwent 5 epochs of training.
- **Problem Solved**: Both models successfully solved the same problem, reaching comparable levels of accuracy.

### Training Time Comparison
| Model         | Training Time |
|---------------|---------------|
| Mamba Model   | 1.32 seconds  |
| Transformer   | 2.39 seconds  |

- **Difference in Training Time**: **1.07 seconds**

### Model Parameter Comparison
| Metric                     | Difference |
|----------------------------|------------|
| Total Parameters           | 1771       |
| Trainable Parameters       | 1771       |

The **Mamba** model demonstrated faster training time and lower parameter count compared to the **Transformer** model, making it a more efficient alternative for tasks that require quick iterations and fewer computational resources, especially for long sequence tasks.

### Summary
- **Efficiency**: The Mamba model trained significantly faster (1.32s vs. 2.39s) compared to the Transformer model.
- **Model Complexity**: The Transformer model had **1771 more parameters** than the Mamba model, which provided better representational capacity but increased the training time and resource requirements.

These results suggest that **Mamba** is a highly efficient option for sequence modeling tasks, particularly in scenarios with limited computational resources or when handling long sequences. However, the Transformer model may still hold an edge for tasks requiring more detailed context due to its richer parameter set.
