# Method note


**Inputs and checks.** Dataset cloned from GitHub (commit `24881cc`): 35,670 rows, 1,125 participants, each seeing one advice label. Two README entries don't match the data: `task_instance_id` is text, not 1–32, and survey order runs 0–31, not 1–32. Answers of exactly 0 (458 before, 681 after) count as no label. The paper's method (arXiv 2107.07015) says the "AI" advice was averaged human answers, except in dermatology; I confirmed in the data that advice accuracy is the same under both labels. QCB section 13 was read from the official scanned PDF. The 81% reproduces as 80.9%, and every figure in the text was checked by script against the notebook output.

**Tools.** Python 3.11 (pandas, numpy, matplotlib), Jupyter in VS Code.

**Time.** Task 1 **145** min, Task 2 ** 30**, Task 3 ** 20** (`TIME_LOG.md`). **Main problems:** the "AI" is mostly not an AI; the Guideline is a scanned PDF; answers are linked within each person, so the intervals resample people. **With more time:** a model with person and item effects, and the dermatology task (real AI) analysed separately.

**Confidence** 
1. Right answers dropped for wrong advice: **85%**. Large samples and narrow intervals; a bank's AI errors may fall on different cases.
2. Confident wrong advice overturns more: **70%**. It holds within the same item, but the strength scale is a survey slider.
3. How the tool is described changes checking: **55%**. Randomised, but from one task with a wide interval.

**Least sure of:** whether crowdworkers on puzzles behave like trained bank reviewers.
