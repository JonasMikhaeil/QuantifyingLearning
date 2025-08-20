# Quantifying How Much Has Been Learned from a Research Study

How much does a research study contribute to a scientific literature? We propose a learning metric to quantify how much a research community learns from a given study. To do so, we adopt a Bayesian perspective and assess changes in the community's beliefs once updated with a new study's evidence. We recommend the Wasserstein-2 distance as a way to describe how the research community's prior beliefs change to incorporate a study's findings. While assessments about what has or could be learned from a research program are often expressed informally, our learning metric provides a principled tool for judging scientific contributions. By formalizing these judgments, our measure has the potential to allow for more transparent assessments of past and prospective research contributions.

## Stylized Example 
In the case of normal prior $\pi_0 = normal(\mu_0,\sigma_0)$ and posterior $\pi_1 = normal(\mu_1,\sigma_1)$, our learning metric is particularly easy to calculate:
$W_2^2(\pi_0,\pi_1) = (\mu_0 - \mu_1)^2 + (\sigma_0 - \sigma_1)^2$ 
The following figure illustrates how much is learned in four scenarious in which a normal(0,10) prior is updated. 
![styl_fig.pdf](https://github.com/user-attachments/files/21907440/styl_fig.pdf)

## Quantyfing learning when distributions are non-normal
Our learning metric can also be applied when prior or posterior are non-normal as the following figure illustrates:
![Green_NonNormalPrior.pdf](https://github.com/user-attachments/files/21907454/Green_NonNormalPrior.pdf)
We provide code for this exampe in QuantyfingLearning.Rmd
