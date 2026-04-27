# Full 90-Language Benchmark

This is a comprehensive multilingual evaluation covering 90 languages, comparing Chandra 2 against Gemini 2.5 Flash. The average scores are lower than the [43-language benchmark](README.md#multilingual-benchmark-table) because this includes many lower-resource languages.

## Overall Scores

| | Chandra 2 | Gemini 2.5 Flash |
|---|:---:|:---:|
| **Average** | **72.7% +/- 1.2%** | **60.8% +/- 1.3%** |

> **Personal note:** Chandra 2 wins on 68 out of 90 languages. Notable weak spots for Chandra 2: `ps` (12.6%), `yi` (24.9%), `ug` (25.8%), and `or` (31.1%). Languages where Gemini 2.5 Flash leads by a significant margin: `su` (+10.7%), `vi` (+6.9%), `ur` (+13.5%).

> **My note:** I'm particularly interested in the South/Southeast Asian language results. The gap on `km` (46.1% vs 6.3%), `lo` (60.9% vs 13.3%), and `my` (55.9% vs 15.8%) is striking — worth digging into whether this is a tokenization or training data issue on Gemini's side.

> **TODO (personal):** Cross-reference the weak `ps`, `yi`, and `ug` scores against training corpus size estimates. I suspect `yi` (Yiddish) underperforms due to script overlap with Hebrew causing tokenization confusion — similar pattern to what I saw in the `he` vs `yi` comparison in my notes.

> **My note:** The `si` row appears to be cut off in the original table — scores are missing. Need to check the source data and fill this in. Same may apply to any languages below `si` that didn't make it into this file.

## Results by Language

| Language | Chandra 2 | Gemini 2.5 Flash |
|----------|:--------:|:----------------:|
| af | 80.4% | 85.8% |
| am | 34.4% | 0.5% |
| ar | 68.4% | 84.4% |
| as | 35.8% | 23.1% |
| az | 75.2% | 74.0% |
| be | 80.7% | 66.4% |
| bg | 83.1% | 64.3% |
| bn | 72.8% | 55.3% |
| br | 90.0% | 69.4% |
| bs | 84.8% | 85.1% |
| ca | 85.1% | 88.0% |
| cs | 85.3% | 79.1% |
| cy | 82.2% | 77.6% |
| da | 91.1% | 86.0% |
| de | 94.8% | 88.3% |
| el | 85.6% | 83.5% |
| en | 96.6% | 90.3% |
| eo | 80.1% | 71.9% |
| es | 89.3% | 86.8% |
| et | 75.2% | 73.7% |
| eu | 80.2% | 74.6% |
| fa | 75.1% | 61.8% |
| fi | 83.4% | 86.0% |
| fr | 93.7% | 86.1% |
| fy | 81.2% | 70.1% |
| ga | 80.9% | 70.1% |
| gd | 71.8% | 59.5% |
| gl | 80.9% | 80.9% |
| gu | 70.8% | 47.6% |
| ha | 72.1% | 59.1% |
| he | 70.4% | 50.9% |
| hi | 78.4% | 82.7% |
| hr | 90.1% | 88.2% |
| hu | 82.1% | 84.5% |
| hy | 64.2% | 42.1% |
| id | 91.6% | 88.3% |
| is | 77.3% | 72.2% |
| it | 94.6% | 85.7% |
| ja | 86.9% | 80.0% |
| jv | 73.2% | 80.4% |
| ka | 77.0% | 39.3% |
| kk | 80.5% | 77.2% |
| km | 46.1% | 6.3% |
| kn | 63.2% | 24.5% |
| ko | 81.5% | 84.8% |
| ku | 62.0% | 63.2% |
| ky | 81.2% | 69.8% |
| la | 73.8% | 70.5% |
| lo | 60.9% | 13.3% |
| lt | 79.8% | 70.5% |
| lv | 76.9% | 81.5% |
| mg | 81.2% | 78.4% |
| mk | 83.5% | 77.4% |
| ml | 64.3% | 23.8% |
| mn | 88.4% | 71.4% |
| mr | 75.0% | 69.7% |
| ms | 79.3% | 79.8% |
| my | 55.9% | 15.8% |
| ne | 45.3% | 43.0% |
| nl | 88.6% | 87.5% |
| no | 90.5% | 87.8% |
| or | 31.1% | 11.2% |
| pa | 48.3% | 22.4% |
| pl | 91.5% | 91.1% |
| ps | 12.6% | 13.3% |
| pt | 95.2% | 89.4% |
| ro | 84.5% | 76.7% |
| ru | 85.5% | 82.8% |
| sa | 51.1% | 44.6% |
| sd | 50.0% | 29.3% |
| si | *(missing — TODO: pull from source data)* | *(missing)* |
