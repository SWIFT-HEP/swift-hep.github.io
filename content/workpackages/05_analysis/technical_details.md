---
title: "Analysis Systems - Technical Details"
mermaid: true
---

## Anatomy of an analysis

{{<mermaid>}}
graph TD 
  d1[data]-->T1[Task]
  d1[data]-->T2[Task]
  d1[data]-->T3[Task]
  T1[Task]-->d2[data]
  T2[Task]-->d2[data]
  T3[Task]-->d3[data]
  d2[data]-->T4[task]
  d2[data]-->T5[task]
  d3[data]-->T5[task]
  T4[Task]-->d4[data]
  T5[Task]-->d4[data]
  d4[data]-->T6[task]
  T6[Task]-->d5[data]  
{{</mermaid>}}
