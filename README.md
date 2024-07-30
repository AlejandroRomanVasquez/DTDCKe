This repository contains the source code for the paper "DERANDOMIZED TRUNCATED D-VINE COPULA KNOCKOFFS WITH E-VALUES TO CONTROL THE FALSE DISCOVERY RATE." 
https://doi.org/10.48550/arXiv.2407.14002

The computational implementations of the proposed methods were carried out using R and Python programming languages, employing versions 3.6.3 and 3.9.7, respectively. 
The code for running the simulations and the application to a real dataset uses several packages from R and Python. The R packages are the following: dplyr (version 1.0.9), glmnet (version 4.1.4), rvinecopulib (version 0.6.2.1.3), knockoff (version 0.3.5), sn(version 2.0.2), doMC (version 1.3.8), foreach (version 1.5.2), doParallel (version 1.0.17), TSP (version 1.2.4), and VineCopula (version 2.4.5). The Python libraries are the following: numpy (version 1.20.3), pandas (version 1.3.4), joblib (version 1.1.0), matplotlib (version 3.4.3), knockpy (version 1.1.1), and rpy2 (version 3.5.1).

The folder "Simulations" contains code related to 4 four distinct data-generating processes (DGPs) for the predictors X considered in the paper: a truncated D-vine copula, a multivariate normal distribution, a t-tailed Markov chain, and a parametric D-vine copula fitted to gene expression data. Each configuration has two Jupyter notebook files, one for Gaussian Linear response and the other for Logistic regression response.

The folder "Application" contains code and data for applying the proposed methodology to a real lung cancer dataset.

As mentioned in the paper, we compare the statistical power and FDR control of five distinct Model-X knockoff methods in our simulations and application to real data: the parametric DTDCKe procedure, the non-parametric DTDCKe procedure, Vineknockoffs (Kurz, 2022), Gaussian knockoffs, and second-order knockoffs. For the Gaussian knockoffs, we utilize the minimum variance-based reconstructability (MVR) knockoffs as described by Spector and Janson (2022). Due to computational time constraints, we decided to separate the simulations for Vineknockoffs from the other competing methods. To distinguish these, we appended the word “Vineknockoffs” to the names of the corresponding files.


References:

Kurz, M. S. (2022). Vine copula based knockoff generation for high-dimensional controlled variable selection. arXiv preprint arXiv:2210.11196.

Spector, A., & Janson, L. (2022). Powerful knockoffs via minimizing reconstructability. The Annals of Statistics, 50(1), 252-276.

Vásquez, A. R., Urbina, J. U. M., Farías, G. G., & Escarela, G. (2024). Derandomized Truncated D-vine Copula Knockoffs with e-values to control the false discovery rate. arXiv preprint arXiv:2407.14002.
