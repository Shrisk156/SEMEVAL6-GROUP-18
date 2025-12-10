# SEMEVAL6-GROUP-18

# Task-6: CLARITY 2026

This repository contains our work on **SemEval Task-6**, part of the CLARITY 2026 challenge. The goal of this task is to automatically detect and classify ambiguity in political question/answer pairs from presidential interviews.  
It uses a two-level taxonomy: high-level clarity vs. ambiguity and nine fine-grained evasion techniques.  
This helps analyze how politicians strategically use evasive language.  
The task supports NLP research in discourse analysis, fact-checking, and dialogue systems.  
It provides a standardized dataset and evaluation framework for political communication analysis at scale.

More information can be found on the attached Research Paper.

**Task Link:** [CLARITY SemEval 2026](https://konstantinosftw.github.io/CLARITY-SemEval-2026/)

## Team Members
- Saiesh Kaul
- Shrisha Shriram Kulkarni
- Swapnil Thatte

## 🚀 Key Features
* **Dataset Explosion:** A data augmentation technique that treats conflicting annotator labels as valid distinct training samples, effectively tripling the training data size to capture subjective ambiguity.
* **Hierarchical Flat-Mapping:** A "bottom-up" inference pipeline that predicts fine-grained evasion types (Task 2) and deterministically maps them to high-level clarity labels (Task 1), ensuring logical consistency.
* **Weighted Loss Optimization:** Implementation of `WeightedCrossEntropy` to penalize misclassification of rare evasion types like *Clarification* and *Partial Answer*.
* **ACL-Ready Paper:** Includes the associated research paper.

## 🛠️ Installation

### Prerequisites
* Python 3.8+
* GPU recommended (Google Colab T4 or NVIDIA local GPU)

### Dependencies
Install the required libraries. **Note:** We explicitly downgrade `numpy` to `<2.0` to prevent conflicts with PyTorch.


