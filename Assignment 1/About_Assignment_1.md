# Graph Theory Assignment

## Topic
**To Construct Real Life Network Synthetically of 10000 Nodes and Discover Meaningful Insights & Visualization using NetworkX and Gephi Tools**

---

## Marks
30 Marks

## Date of Submission
10th May 2026

---

# Assignment Details with Marking Scheme

## Part I: Synthetic Real-Life Network Construction using Kronecker Graphs
**Marks: 5**  
**Course Outcome: CO2**

Construct a synthetic real-life network containing **10,000 nodes** using **Kronecker Graph Generation** with the help of the **NetworkX Python Package**.

### Tasks
- Generate a Kronecker Graph
- Ensure the graph simulates properties of real-world networks
- Export the graph into `.gexf` format for Gephi visualization

---

# Part II: Using NetworkX Python Package

## a) Visualization of Real-Life Network
**Marks: 7.5**  
**Course Outcome: CO1**

Draw and visualize the generated network using various NetworkX layouts.

### Requirements
- Create aesthetic graph visualizations
- Use meaningful color combinations and node sizing
- Visualize complete graph and subgraphs
- Apply different layouts such as:
  - Spring Layout
  - Circular Layout
  - Kamada-Kawai Layout
  - Shell Layout
  - Spectral Layout

### Suggested Visualizations
- Degree-based node coloring
- Community-based clustering visualization
- Highlight central nodes
- Dense vs sparse region comparison

---

## b) Calculate Network Insights
**Marks: 7.5**  
**Course Outcome: CO3**

Calculate and analyze the following graph metrics:

### Required Metrics
1. Radius
2. Diameter
3. Average Degree
4. Average Clustering
5. Clustering Coefficient
6. Closeness Centrality
7. Betweenness Centrality
8. Community Detection
9. Modularity

### Expected Analysis
- Interpret each metric
- Explain what the metric reveals about the network
- Compare dense and sparse communities
- Identify influential nodes

---

# Part III: Using Gephi Tool

## a) Visualization using Gephi
**Marks: 7.5**  
**Course Outcome: CO1**

Import the generated `.gexf` file into Gephi and create meaningful visualizations.

### Requirements
- Use various Gephi layouts such as:
  - ForceAtlas2
  - Fruchterman Reingold
  - Yifan Hu
- Apply node coloring and sizing
- Generate subgraph/community visualizations
- Create aesthetically pleasing layouts

### Suggested Enhancements
- Color nodes based on modularity classes
- Size nodes using PageRank or Degree
- Use filters for subgraph extraction

---

## b) Calculate Insights using Gephi
**Marks: 2.5**  
**Course Outcome: CO3**

Calculate the following metrics using Gephi:

### Required Metrics
1. Average Degree
2. Network Diameter
3. Graph Density
4. HITS Algorithm
5. PageRank

### Expected Output
- Metric tables
- Screenshots of statistics panels
- Interpretation of results

---

# Deliverables

## 1. Report (PDF Format)
The report must include:
- Part I implementation
- Part II analysis
- Part III Gephi analysis
- Screenshots of outputs and visualizations
- Insights and interpretations

### Format
`.pdf`

---

## 2. Graph File
Exported graph file.

### Format
`.gexf`

---

## 3. Python Notebook
Implementation notebook containing:
- Graph generation
- Visualization
- Metric calculations

### Format
`.ipynb`

---

## 4. Gephi Project File
Gephi project containing:
- Imported graph
- Layouts
- Statistics
- Filters

### Format
`.gephi`

---

# File Naming Convention

GT_Assign_<your_prn_no>.pdf

GT_Assign_<your_prn_no>.gexf

GT_Assign_<your_prn_no>.ipynb

GT_Assign_<your_prn_no>.gephi

---

# Suggested Python Workflow

1. Generate Kronecker Graph
2. Store graph using NetworkX
3. Compute graph metrics
4. Visualize graph using multiple layouts
5. Export graph to `.gexf`
6. Import into Gephi
7. Apply layouts and statistics
8. Capture screenshots for report

---

# Tools & Technologies

## Python Libraries
- NetworkX
- NumPy
- Matplotlib
- Pandas
- python-louvain

## Visualization Tool
- Gephi

---

# Expected Learning Outcomes

By completing this assignment, students will learn:
- Synthetic graph generation
- Real-world network modeling
- Network visualization techniques
- Graph metric analysis
- Community detection
- Centrality analysis
- Gephi-based graph exploration

---

# References

- NetworkX Documentation  
  https://networkx.org/

- Gephi Official Website  
  https://gephi.org/

- Kronecker Graph Research  
  Leskovec et al. - Kronecker Graphs