# Kernel Density Lab

An interactive study guide for §16.3 of Kevin P. Murphy, *Probabilistic Machine Learning: An Introduction*
(kernel density estimation, KNN from KDE, and kernel regression).

**Live:** https://isaackrallison.github.io/kernel-density-estimation/

Every section has an **Explain it** box at four levels (Kid, High school, Undergrad, Grad / MLE), switchable globally from the top bar.

- **16.3.1 Density kernels:** boxcar, Epanechnikov, tri-cube and Gaussian with a bandwidth slider. The area (Eq. 16.28) and mean (Eq. 16.25) are checked numerically. Includes Figure 16.8, Table 16.1, and a 2-D RBF heat map (Eqs. 16.29–16.30).
- **16.3.2 Parzen window estimator:** build a KDE from the six points of Figure 16.9. Add, drag or erase points, show each bump, and see p(x*) summed term by term. Sample new data from the KDE and watch the histogram converge.
- **16.3.3 Bandwidth:** four known truths (Gaussian, bimodal, lopsided, heavy-tailed t), the rule of thumb with std and with 1.4826·MAD, and ISE and leave-one-out log-likelihood curves over h.
- **16.3.4 From KDE to KNN:** a balloon window with unequal class sizes. The table computes every term of Eq. 16.35 so you can watch N_c and V(x) cancel, with a fixed-radius window to compare.
- **16.3.5.1 Nadaraya-Watson:** kernel regression on noisy sinc data (Figure 16.10), with per-point weights at a draggable query.
- **16.3.5.2 Predictive variance:** a µ ± 2√V band (Eq. 16.45) on constant or growing noise.
- **16.3.5.3 Locally weighted regression:** local constant vs local linear fits, boundary bias, and Eq. 16.46 shown as p̂(x)·µ(x).
- Step-by-step math for Eqs. 16.25–16.47, a 40-question quiz tagged by level, and a cheat sheet.

Single self-contained `index.html`, no build step. Loads Google Fonts and MathJax from cdnjs. All data are synthetic and generated in the page from fixed seeds.
