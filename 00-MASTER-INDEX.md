# PL-300 - Microsoft Power BI Data Analyst Associate - Visual Study Guide

> Concept-only study aid. No exam questions reproduced. Source PDF (if any) stays local + gitignored.

**Skills outline:** https://learn.microsoft.com/credentials/certifications/resources/study-guides/pl-300

## Concept mindmap

```mermaid
mindmap
  root((PL-300))
    Prepare Data
      Sources files DB services
      Storage modes Import DQ Dual Live
      Power Query M
      Profile clean transform
      Append Merge query folding
    Model Data
      Star schema
      Relationships cardinality cross-filter
      DAX measures calc columns VAR
      Time intelligence Date table
      RLS OLS Performance Analyzer
    Visualize and Analyze
      Visual selection
      Bookmarks drillthrough tooltips
      Sync slicers paginated mobile
      AI visuals Key Influencers Decomp Tree
      Q and A anomaly clustering
    Deploy and Maintain
      Workspaces and roles
      Apps subscriptions alerts
      Gateway scheduled refresh
      Promoted Certified content
      Deployment pipelines
```

## Domain map

```mermaid
flowchart LR
    Master["PL-300 Master Index"]
    D01["Prepare the Data"]
    Master --> D01
    D02["Model the Data"]
    Master --> D02
    D03["Visualize and Analyze the Data"]
    Master --> D03
    D04["Deploy and Maintain Assets"]
    Master --> D04
```

## Domain weights

```mermaid
pie showData
    title PL-300 domain weights
    "Prepare the Data" : 27
    "Model the Data" : 30
    "Visualize and Analyze the Data" : 25
    "Deploy and Maintain Assets" : 18
```

> Click a slice / legend label to jump to that chapter.

## Recommended study order

```mermaid
gantt
    title Suggested study plan
    dateFormat X
    axisFormat Day %d
    section Plan
    Prepare the Data :t1, 0, 1d
    Model the Data :t2, after t1, 2d
    Visualize and Analyze the Data :t3, after t2, 1d
    Deploy and Maintain Assets :t4, after t3, 1d
```

---

**Next:** open [01-prepare-data.md](01-prepare-data.md)

<!-- TODO: fill remaining sections via Copilot chat. Target structure mirrors c:\az305\study-guide\00-MASTER-INDEX.md. -->
