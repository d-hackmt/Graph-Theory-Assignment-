# Graph Theory Assignments — PRN 25039001007

Coursework submissions for the Graph Theory course covering synthetic network construction, graph analytics, and graph database modelling.

---

## Assignments

### [Assignment 1](Assignment%201/README.md) — Synthetic Network Construction & Analysis
> Construct a 10,000-node real-life network using Kronecker Graphs and derive insights using NetworkX and Gephi.

- **Marks:** 30
- **Tools:** Python (NetworkX, Matplotlib, python-louvain), Gephi
- **Key work:** Kronecker graph generation · 5 layout visualisations · 9 network metrics · Gephi layouts + statistics

### [Assignment 2](Assignment%202/README.md) — Graph Database Modelling & Insights
> Model the Global Superstore dataset as a property graph in Neo4j and derive two complex graph analytics insights.

- **Marks:** 20
- **Tools:** Neo4j AuraDB, Cypher
- **Key work:** 4-node graph schema · CSV import (43,836 nodes, 156,848 relationships) · 2 GDS insights

---

## Folder Structure

```
graph_theory_assignment1/
│
├── README.md
├── requirements.txt
│
├── Assignment 1/
│   ├── About_Assignment_1.md          ← Assignment details & marking scheme
│   └── OUTPUTS/
│       ├── GT_Assign_25039001007.pdf
│       ├── GT_Assign_25039001007.ipynb
│       ├── GT_Assign_25039001007.gexf
│       ├── GT_Assign_25039001007.gephi
│       ├── GT_Assign_25039001007.docx
│       ├── Gephi outputs/             ← Gephi layout & statistics screenshots
│       ├── IPYNB outputs/             ← NetworkX visualisation outputs
│       └── network_metrics_summary.csv
│
└── Assignment 2/
    ├── About ASSIGNMENT2.md           ← Assignment details & marking scheme
    ├── superstore data/
    │   └── superstore.csv             ← Dataset (51,290 rows)
    └── Assignment Solution/
        ├── Screenshots/               ← Neo4j query & graph screenshots
        ├── csv outputs/               ← Exported query result tables
        └── Submission Files/
            ├── GT_MiP_25039001007.docx
            ├── GT_MiP_25039001007.pdf
            └── GT_MiP_25039001007.txt
```
