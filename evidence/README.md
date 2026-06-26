# Evidence Summary

## RAGAS comparison

Prompt V1 achieved higher faithfulness and answer relevancy:

- Faithfulness: V1 `0.9645`, V2 `0.9426`
- Answer relevancy: V1 `0.9127`, V2 `0.8895`
- Context recall: both `1.0000`
- Context precision: V1 `0.9450`, V2 `0.9417`

V1 likely performs better on faithfulness because it is shorter and more restrictive: it asks the model to answer only from context and avoid speculation. V2 produces more structured answers, which slightly improves context precision but introduces more wording and therefore more chances for unsupported claims.

## Required evidence files

- `01_langsmith_traces.png`
- `02_prompt_hub.png`
- `02_ab_routing_log.txt`
- `03_ragas_scores.png`
- `03_ragas_report.json`
- `04_pii_demo_log.txt`
- `04_json_demo_log.txt`
