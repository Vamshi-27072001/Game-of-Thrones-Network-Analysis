# Game of Thrones Network Analysis

## Project Overview

This project analyzes the co-occurrence network of characters from the Game of Thrones book series, written by George R.R. Martin. The analysis is performed using network science techniques to uncover the relationships and importance of various characters throughout the books. Characters are considered to co-occur if their names appear within 15 words of each other.

## Dataset

The dataset, named `game.csv`, contains the following columns:

- Source: The name of the first character in the relationship.
- Target: The name of the second character in the relationship.
- Type: The type of relationship (all edges are undirected).
- Weight: The number of interactions between the two characters.
- Book: The specific book in the series (e.g., Book 1, Book 2, etc.).
  
## Objectives
The main objectives of this analysis are to:

1. Create a co-occurrence network using NetworkX.
2. Calculate various centrality measures to determine character importance.
3. Visualize the top characters based on their degree centrality and other metrics.

## Requirements

To run this analysis, you'll need:

- Python
- Libraries:
  - `pandas`
  - `networkx`
  - `matplotlib`
  - `sqlalchemy`
  - `pymysql`
##### Prepare the Environment: Make sure you have all required packages installed (as listed above).
## Analysis Details
- Co-occurrence Network Creation
- The analysis begins by loading the dataset into a pandas DataFrame.
-Using the networkx library, an undirected graph is created where nodes represent characters and edges represent co-occurrences.
## Centrality Measures.

The following centrality measures are calculated to assess character importance:

- Degree Centrality: Measures the number of direct connections (neighbors) a character has.
- Closeness Centrality: Measures how quickly a character can access other nodes in the network.
- Eigenvector Centrality: Considers not just the number of connections but the quality and importance of those connections.
- Betweenness Centrality: Measures how often a character acts as a bridge along the shortest path between two other characters.
- Clustering Coefficient: Indicates how connected a character's neighbors are to each other.

## Visualizations
The following visualizations are generated during the analysis:

- Top 10 Characters Based on Degree Centrality: A bar chart displaying the degree centrality of the top 10 characters.
- Subgraph of Top 10 Characters: A network graph showing the relationships between the top 10 characters based on degree centrality.
- These visualizations are saved in the visualizations folder as PNG files.
## Conclusion
This analysis provides insights into the character relationships within the Game of Thrones series
