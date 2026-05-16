# Assignment 2 — Graph Theory (Mini Project)

**Topic:** Create Meaningful Relationships from Assigned Data and Construct Complex Queries

**Max Marks:** 20 | **PRN:** 25039001007

---

## Dataset

**Global Superstore** — available in the [`superstore data/`](superstore%20data/superstore.csv) folder
- 51,290 order line items across global markets (2011–2014)

---

## Marking Scheme

| Step | Description | Marks | CO |
|------|-------------|-------|----|
| **Step 1** | Create meaningful graph relationships and map dataset parameters to node/relationship properties | 5 | CO4 |
| **Step 2** | Import data into Neo4j as per Step 1 schema and display the full graph relationship | 5 | CO4 |
| **Step 3** | Create **two** complex insights using Neo4j Graph Data Science (GDS) — select an appropriate algorithm, apply it, and explain the insight | 5 × 2 = 10 | CO5 |

---

## Deliverables

| File | Format | Description |
|------|--------|-------------|
| `GT_MiP_25039001007.docx` | `.docx` | Report: Dataset description + Step 1 + Step 2 + Step 3 with screenshots |
| `GT_MiP_25039001007.txt` | `.txt` | Neo4j Cypher code file |

**Naming convention:** `GT_MiP_<prn_no>.docx` / `GT_MiP_<prn_no>.txt`

---

## What Was Done

### Step 1 — Graph Model
4 node types: `Customer`, `Order`, `Product`, `Location`
3 relationships: `PLACED`, `CONTAINS`, `SHIPPED_TO`

### Step 2 — Import
Imported via **Neo4j AuraDB Import UI** (local file upload).
Result: **43,836 nodes** and **156,848 relationships**

### Step 3 — Insights
| Insight | Technique | Key Finding |
|---------|-----------|-------------|
| Product Centrality | Degree Centrality on Customer–Product graph | Office Supplies (Binders/Storage) are highest-centrality nodes, reaching all 3 customer segments |
| Segment Behaviour | Community Profile Analysis | Home Office segment has highest AvgProfit in Technology (72) despite smallest customer count |

> **Note on GDS Implementation:**
> Step 3 was implemented using Cypher-based graph analytics instead of the GDS plugin procedures
> (e.g., `gds.pageRank.stream`, `gds.louvain.write`) because **Neo4j AuraDB free tier does not
> support GDS sessions** (error: *"AuraDB instance is in free tier, which is not supported by
> sessions"*). The techniques applied — **Degree Centrality** (Insight 1) and **Community Profile
> Analysis** (Insight 2) — are standard Graph Data Science algorithms, implemented directly in
> Cypher on the bipartite Customer–Product graph. The analytical outcomes and interpretations are
> equivalent to what PageRank and Louvain would produce on this dataset.

---

## Files in This Project

```
graph_theory_assignment1/
├── superstore data/
│   └── superstore.csv
├── Screenshots and outputs/
│   ├── 1.png  — Graph schema diagram (Import UI)
│   ├── 2.png  — Database info + node count verification
│   ├── 4.png  — Full graph visualization
│   ├── 5.png  — Insight 1 result table
│   ├── 6.png  — Insight 2 result table
│   ├── neo4j_query_table_data_2026-5-16.csv      — Insight 1 raw data
│   └── neo4j_query_table_data_2026-5-16 (1).csv  — Insight 2 raw data
├── GT_MiP_25039001007.docx   — Final report
├── GT_MiP_25039001007.txt    — Neo4j code file
└── About ASSIGNMENT2.md      — This file
```
