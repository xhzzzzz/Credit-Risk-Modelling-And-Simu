# Credit-Risk-Modelling-And-Simulations

The purpose of this assignment is to model a credit-risky portfolio of corporate bonds. Consider a structural model for portfolio credit risk described in class. Using the data for 100 counterparties, simulate 1-year losses for each corporate bond. You will need to generate 3 sets of scenarios:

• Monte Carlo approximation 1 : 5000 in-sample scenarios (N = 1000 · 5 = 5000 (1000 systemic
scenarios and 5 idiosyncratic scenarios for each systemic), non-Normal distribution of losses);

• Monte Carlo approximation 2 : 5000 in-sample scenarios (N = 5000 (5000 systemic scenarios
and 1 idiosyncratic scenario for each systemic), non-Normal distribution of losses);

• True distribution: 100000 out-of-sample scenarios (N = 100000 (100000 systemic scenarios
and 1 idiosyncratic scenario for each systemic), non-Normal distribution of losses).

The out-of-sample scenarios represent true distribution of portfolio losses. Two in-sample non-
Normal datasets are used for evaluating sampling error and performing portfolio optimization.

To evaluate model error (if we wrongly assumed that counterparty losses follow Normal distri-
bution), compute mean loss and standard deviation of losses for each corporate bond from the
3 scenario sets (N =1000×5, 5000, 100000). This 3 in-sample sets are referred as in-sample Normal
model.

Evaluate VaR and CVaR at quantile levels 99% and 99.9% for the two portfolios:
(1) one unit invested in each of 100 bonds;
(2) equal value (dollar amount) is invested in each of 100 bonds;

For each portfolio, compute VaR and CVaR at quantile levels 99% and 99.9% for each of the six
datasets (non-Normal with N =1000×5, 5000, 100000; and Normal with mean/standard deviation
computed from N =1000×5, 5000, 100000). Compare each in-sample VaR and CVaR to out-of-
sample VaR and CVaR. Explain the effects of sampling error and model error.

To better evaluate sampling and model errors, perform the experiment 100 times in the following
way: generate in-sample datasets with N =1000×5 and 5000 (non-Normal and Normal) one hundred
times and compute VaR and CVaR. Keep the out-of-sample scenario set unchanged. Perform
analysis of the results for the 100 trials, e.g., compute averages of the results for 100 trials, analyze
standard deviation over 100 trials, etc.
