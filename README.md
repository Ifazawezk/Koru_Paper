# Does oversight work?

Koru Impact work sample, October 2026.

| File | What it is |
|---|---|
| `task1_oversight.ipynb` | Task 1: code, figures and answers to questions 1 to 4 |
| `METHOD_NOTE.md` | Task 3: method note |
| `TIME_LOG.md` | Time log |
| `board_page.pdf`, `board_page.docx` | Task 2: one page for the board (also sent by email) |
| `data/haiid_dataset.csv` | The dataset (copy of commit `24881cc`), read by the notebook |
| `data/haiid_dataset_description.csv` | Column descriptions from the dataset repo |
| `data/LICENSE-haiid.txt` | MIT licence of the dataset |

## Re-running

1. The dataset is included in `data/` (commit `24881cc` of github.com/kailas-v/human-ai-interactions, 27 Oct 2022, 35,670 rows).
2. Install Python 3.11 and run `pip install -r requirements.txt`.
3. Open `task1_oversight.ipynb` and choose Run All. It takes under a minute. The resampling uses a fixed seed, so the intervals come out the same on every run.

## Sources

- Vodrahalli, K., Daneshjou, R., Gerstenberg, T. and Zou, J. (2022). Do humans trust advice more if it comes from AI? AIES '22, 763–777. Method read from arXiv 2107.07015.
- Dataset: github.com/kailas-v/human-ai-interactions, MIT licence, copyright (c) 2022 Kailas Vodrahalli.
- Qatar Central Bank (2024). Artificial Intelligence Guideline, Part C, section 13. In force 4 Sep 2024. PDF from https://www.qcb.gov.qa/Services/Financial%20Technology/QCB_Artificial_Intelligence_Guideline.pdf, read 18 Oct 2026.
