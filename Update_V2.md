Following our initial notice in `Update.md`, we performed a further verification of our theoretical derivations, LaTeX tables, and appendix descriptions while preparing the revised preprint. We would like to note the following additional typographical errors and theoretical clarifications:

1. Notation & Formula Typographical Errors:
   - Hyperbolic Distance & Logarithmic Map: Due to a typographical error in the LaTeX text, the negative sign was misplaced. 
   
     *(Note: Our actual code implementation calls the standard Manify library backend and is unaffected by this text typo.)*
   - Intermediate Gradient Exponent: In the second line of Eq. (84), the exponent inside the parentheses was mistyped as $-2/(m-1)$ instead of $+2/(m-1)$. The final gradient formula in Eq. (11) are correct, and our implementation is accurate as well.

2. Table Transcription & Typographical Errors:
   
   - Table 8 ($F_1$ Entries for RFK): The $F_1$ entries for RFK on CiteSeer (recorded as 0.07) and Cora (recorded as 0.06) were transcription errors during table entry, their correct values are 6.71 and 6.46, respectively. The baseline entries in those rows are unaffected.
   - Table 2: Due to a manual transcription error when compiling the table from raw logs, the `Min` and `Last` loss values for MNIST under RAdam were inverted. The  entries for Gauss $R^2S^2H^2$ and $S^2(H^2)^2$ in Table 1 were transposed.

3. Appendix Metric & Textual Clarifications:
   - Metric Implementations: In Appendix D.2 describe pairwise $F_1$ in the text, whereas the evaluation script first performs Hungarian label alignment itself, and then calls the standard scikit-learn implementation of macro-F1 on the aligned labels.

---

Corrections for all items in both `Update.md` and `Update_v2.md` will be incorporated together into the revised version of the preprint (v2). Until that revision is released, these two notes serve as our complete correction notice.