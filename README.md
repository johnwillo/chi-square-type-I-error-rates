# Examination of type I error rates of chi-square tests of 2x2 contingency table data
This paper examines how well the chi-square test on a 2x2 contingency table approximates the desired Type I error (alpha) specified for the test through simulations. The results for equal and unequal sample sizes are examined, as well as for varying levels of probability. The use of the Yates' correction for continuity is also explored. Yates' correction for continuity is often employed in the case of 2x2 contingency tables, and R's chisq.test() function applies the correction by default to a 2x2 table. But many authors have pointed out that the correction is too conservative; see, for example, Amiri and Modarres (2017).

For a binomial probability of 0.01, observed type I error rates are not even close to 0.05 until the sample size reaches 500, in which case the uncorrected type I error is close to 0.05. When the probability is increased to 0.05, robustness is not achieved until the sample size is 100 for both samples and the uncorrected type I error becomes close to 0.05. For probabilities of 0.10 and above, the uncorrected type I error rate is close to 0.05 and therefore robust.
