# engagemii-index-free-sample

Free data on how visible companies are to AI assistants (ChatGPT, Claude, Perplexity, Gemini and others).

This repo holds a 500-company US sample from the Engagemii Index, the world's largest AI visibility index. The index scores 82 million+ companies on how visible they are to AI assistants. Engagemii logs which AI engines read about each company and how often.

## What is in the sample

500 US companies, one row each, with every field Engagemii holds:

- AI visibility score
- Which AI engines read about the company and how often
- Industry
- Location
- Tech stack
- Business relationships on record

## Files

| File | What it is |
|---|---|
| `engagemii-index-sample-500.csv` | The 500-company sample, one row per company |
| `columns.md` | The 113 column names, in file order |
| `LICENSE` | CC BY 4.0 |

## How to use

```python
import pandas as pd
df = pd.read_csv("engagemii-index-sample-500.csv")
print(df.sort_values("aeoScore", ascending=False).head(10))
```

A few things people do with it:

- Match it against a lead list to see which leads AI assistants can actually find
- Group by industry or location and compare AI visibility
- Look at which AI engines read about which kinds of companies

## The 1 million company list

A larger free list covers 1 million companies with four columns: website, AI visibility level (High/Medium/Low), whether AI engines read about the company in the last 30 days, and whether it has business relationships on record.

Get either dataset here:

- https://engagemii.com/sample (work email required)
- Databricks Marketplace, 500 sample: https://marketplace.databricks.com/details/528dc208-d86f-46f3-b29f-f79b9d45074d/Engagemii_Engagemii-AI-Visibility-US-Companies-Free-Sample
- Databricks Marketplace, 1 million list: https://marketplace.databricks.com/details/4ac9af6a-667c-4fa3-9534-45402ef73108/Engagemii_Engagemii-Index-1-Million-Companies-Free

## License

CC BY 4.0. Credit "Data from the Engagemii Index, https://engagemii.com" when you use it.

## Claim your company page

Every company in the Engagemii Index has a free public page on engagemii.com. If one of them is yours, go to engagemii.com, find your company, and claim the page.
