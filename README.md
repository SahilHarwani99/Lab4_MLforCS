# Lab4_MLforCS
# Project Title

## Overview
This project focuses on countering backdoor vulnerabilities in neural networks, specifically BadNets trained on the YouTube Face dataset. The objective is to design GoodNet, a model capable of accurately classifying clean inputs while detecting and labeling backdoored inputs as an additional category.

## Data
The YouTube Aligned Face Dataset serves as the foundation, split into 'valid.h5' for validation and 'test.h5' for evaluating the pruned network's effectiveness.

## Procedure
- **Defense Mechanism:** Utilizes channel pruning from BadNet's conv_3 layer, guided by clean validation set metrics.
- **GoodNet Design:** Compares outputs between the pruned model (B') and original BadNet (B) to identify discrepancies for backdoor detection.

## Observations
- **Channel Pruning Impact:** Highlights a trade-off between increased security (reduced attack success rate) and reduced accuracy on clean data.
- **Performance Table:** Demonstrates the correlation between increased pruning and decreased attack success rate, emphasizing the trade-offs involved. Exact values can be found in the report.

## Code Execution Notes
- Ensure all dependencies are installed with latest versions.
- Upload the data on your drive and make sure the paths are correctly updated.
- Set accurate path directories for clean data, poisoned data, models, and saved model states.


## Conclusion
The project highlights the delicate balance between security measures and model performance in neural network design. Channel pruning exhibits potential to enhance security against backdoor attacks while impacting accuracy on clean data. Insights gained from this study contribute to implementing defenses in neural network architectures, acknowledging the inherent trade-offs.
