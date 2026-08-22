# Dice Is Quadratic, Jaccard Is Exponential: Convex Calibration of Set Similarities

## Abstract

Dice and Jaccard are monotone transforms on each prediction-outcome pair, yet their statistically calibrated convex surrogates have radically different dimension. For $s$-label instance-wise prediction, recent work places the convex calibration dimension of Dice/F1 at order $s^2$. We prove that Jaccard loss instead satisfies

$$2^{s-1}\ \leq\ \mathrm{CCdim}(L^{\rm Jac})\ \leq\ 2^s-1.$$

Thus every distribution-free convex calibrated surrogate for example-based intersection over union needs exponentially many prediction coordinates. The score and loss matrices both have exact rank $2^s$, and the loss has affine dimension $2^s-1$. The lower bound is not a rank argument. We construct a full-support outcome law for which exactly $2^{s-1}+1$ reports are Bayes optimal: the empty report and all reports containing one distinguished label. Its boundary form combines an empty-outcome atom with factorial mass proportional to $1/(|A|-1)!$ on sets containing that label. A factorial cancellation makes all active reports tie, while strict positive definiteness of the Jaccard kernel makes their loss columns affinely independent. The feasible-subspace theorem then gives the lower bound. We also give a self-contained strict-definiteness proof by minwise hashing and Mobius inversion, an explicit calibrated upper surrogate, and a regret transfer. The result explains why low-dimensional convex IoU extensions cannot be exactly calibrated without additional assumptions.

## Keywords

dice, quadratic, jaccard, exponential, convex, calibration, similarities, monotone, transforms

## Files

- `main.pdf`, `supplement.pdf`
- `main.tex`, `supplement.tex`
- `references.bib`
- `aistats2027.sty`, `fancyhdr.sty`
- `main.pdf.ots`, `supplement.pdf.ots`, `README.md.ots` OpenTimestamps priority proofs
