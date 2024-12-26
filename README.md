# Frequent Pattern Mining with Apriori & FP-Growth
 This project implements Apriori and FP-Growth algorithms for frequent pattern mining and association rule generation. It processes transactional datasets to discover frequent itemsets and extract insights using support and confidence thresholds. Both algorithms are optimized for performance and usability in real-world data mining tasks.

# Frequent Pattern Mining: Apriori & FP-Growth

This project provides an implementation of two popular data mining algorithms: **Apriori** and **FP-Growth**. These algorithms are used for discovering frequent itemsets and generating association rules from transactional datasets, commonly applied in market basket analysis and recommendation systems.

## Features

- **Apriori Algorithm**:
  - Iterative generation of candidate itemsets.
  - Support-based pruning to filter infrequent itemsets.
  - Extraction of association rules based on minimum confidence.

- **FP-Growth Algorithm**:
  - Efficient construction of an FP-Tree for compressing transaction data.
  - Recursive mining of conditional FP-Trees to find frequent itemsets.
  - Association rule generation from mined patterns.

## Input Requirements

- **Dataset**: A CSV file containing transactional data with the following columns:
  - `CID`: Customer ID.
  - `IiD`: Item ID.
  - `PName`: Product Name.
- **Parameters**:
  - **Minimum Support**: Filters out itemsets appearing less frequently than this threshold.
  - **Minimum Confidence**: Ensures rules meet the minimum confidence level.

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name




Running Apriori Algorithm...
Frequent Itemsets:
[('A',), ('B',), ('A', 'B')]

Association Rules:
('A',) -> ('B',) [support: 0.5, confidence: 0.8]

Running FP-Growth Algorithm...
Frequent Itemsets:
['A'], ['B'], ['A', 'B']

Association Rules:
['A'] -> ['B'] [support: 0.5, confidence: 0.8]
