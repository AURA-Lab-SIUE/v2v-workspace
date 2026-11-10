# 03_Data

Notes on your data, from Chapters 10 to 12: where it came from, how you drew your sample,
and any terms it came with.

The data files themselves go in `data/` at the top of the workspace, beside `README.md`.
The course guides' R code points there, such as `read_csv("data/coding-form.csv")`, and the
AURA Lab R Companion saves your reliability codes in `data/derived/`.

Keep the raw sample and your coded output as separate files in `data/`. Never edit the raw
sample in place; if you do, you cannot show anyone how you got from it to your results.

**Do not commit data you are not licensed to redistribute.** If a dataset came with
terms, respect them. Course practice data comes from the `v2v` package, so you do not
need to commit that at all; load it with `library(v2v)`.
