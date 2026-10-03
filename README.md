# Automated Cultural Content Classification in EFL Textbooks

## Overview

This repository contains the research dataset associated with the study:

**Automated Cultural Content Classification in EFL Textbooks: An Imbalance-Aware ELECTRA Framework with LLM-Based Augmentation**

The study investigates automated classification of cultural representations in English as a Foreign Language (EFL) textbooks used under Indonesia's Merdeka Curriculum. The dataset was developed from eight English textbooks covering Grades III, IV, V, VI, VII, VIII, IX, and XI.

Text extracted from the textbooks was cleaned, segmented, and manually annotated for cultural representation. The resulting dataset contains **2,195 text segments**.

## Cultural Categories

Each text segment was classified into one of four categories:

| Label | Category | Description |
|---|---|---|
| NC | Non-Cultural | Segments containing no specific cultural representation |
| SC | Source Culture | Cultural representations of Indonesia, including national and local cultures |
| IC | International Culture | Cultural representations of countries other than Indonesia and English-speaking countries |
| TC | Target Culture | Cultural representations of English-speaking countries |

The annotation framework is based on the cultural classification proposed by Cortazzi and Jin (1999).

## Dataset Summary

The final annotated dataset contains 2,195 text segments with the following class distribution:

| Category | Number of Segments | Percentage |
|---|---:|---:|
| Non-Cultural (NC) | 1,811 | 82.51% |
| Source Culture (SC) | 280 | 12.76% |
| International Culture (IC) | 88 | 4.01% |
| Target Culture (TC) | 16 | 0.73% |
| **Total** | **2,195** | **100%** |

Three annotators independently annotated the text segments. Final labels were determined using majority voting. Inter-annotator agreement was assessed using Fleiss' Kappa.

## Repository Structure

```text
Automated-Cultural-Content-Classification-in-EFL-Textbooks/
│
dataset/
├── final_annotated_dataset.csv
├── train_dataset.csv         
├── test_dataset.csv          
└── augmented_data/   
│
├── README.md
├── LICENSE
└── CITATION.cff
