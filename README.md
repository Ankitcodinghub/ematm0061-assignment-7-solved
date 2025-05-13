# ematm0061-assignment-7-solved
**TO GET THIS SOLUTION VISIT:** [EMATM0061 Assignment 7 Solved](https://www.ankitcodinghub.com/product/ematm0061-assignment-7-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93033&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EMATM0061 Assignment 7 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Introduction

This document describes your sixth assignment for Statistical Computing and Empirical Methods (Unit EMATM0061) on the MSc in Data Science. Before starting the assignment it is recommended that you first watch video lectures 15, 16, 17.

Begin by creating an Rmarkdown document with html output. You are not expected to hand in this piece of work, but it is a good idea to get used to using Rmarkdown.

1 Student’s t-confidence intervals

In this problem we will discuss a parametric approach to obtaining confidence intervals based upon Student’s t-distribution. In the code below “adelie_flippers” is a vector containing the flipper lengths of a sample of Adelie penguins. The following code computes confidence intervals based on “adelie_flippers” for the population mean of the flipper lengths for Adelie penguins using the Student’s t-distribution method.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>alpha&lt;-0.05
sample_size&lt;-length(adelie_flippers)
sample_mean&lt;-mean(adelie_flippers)
sample_sd&lt;-sd(adelie_flippers)
t&lt;-qt(1-alpha/2,df=sample_size-1)
confidence_interval_l&lt;-sample_mean-t*sample_sd/sqrt(sample_size)
confidence_interval_u&lt;-sample_mean+t*sample_sd/sqrt(sample_size)
confidence_interval&lt;-c(confidence_interval_l,confidence_interval_u)
confidence_interval
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
What would happen to the width of my confidence interval if the sample mean were higher? What would happen to the width of my confidence interval if the sample standard deviation were higher? What would happen to the width of my confidence interval if the sample size were larger?

Use your data wrangling skills to extract a vector consisting of the weights of all the Red-Tailed hawks from the “Hawks” data set, with any missing values removed.

Now use the Student’s t method to compute 99%-level confidence intervals for the population mean of the weights for the red tailed hawks. Note that opting for confidence intervals with a confidence level of 99%, rather than a confidence level of 95%, requires a modified value of α.

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
What assumptions are made to derive confidence intervals based on Student’s t-distribution? Check if these assumptions are justified using a kernel density plot with the geom_density() function and using a QQ-plot with the stat_qq() function.

2 One sample t-test

Begin by loading the “Palmer penguins” library. Next extract a vector called “bill_adelie” consisting of the bill lengths of the Adelie penguins belonging to the Adelie species.

Carry out a statistical hypothesis test to test the hypothesis that the population mean of the Adelie penguin’s bill lengths is 40mm. Use a significance level of 0.01. You can use the t.test() function. What assumptions are required for this hypothesis test?

3 Implementing a one-sample t-test

Implement a function carries out a two sided one-sample t-test. Your sample should take in two arguments 1) a vector x corresponding to a sample X1, · · · , Xn ∼ N (μ, σ2) and a 2) the value μ0 corresponding to a null hypothesis of μ = μ0. The output of your function should be the corresponding p-value of the test.

You can test your implementation by confirming your function gives the same p-value as the t.test() function for the example in question 2 of the assignment.

4 The paired t-test

The Barley data set gives the yields of two types of barley – Glabron and Velvet across twelve different fields. The data is paired as yields are given for both types of barley across each of the twelve fields.

Carry out a paired t-test to determine whether there is a difference in average yield between the two types of barley. Use a significance level of 0.01. You can use the t.test() function.

Compute the effect size using Cohen’s d statistic.

What assumptions are required for the one-sample t test? Are these assumptions justified in this case?

5 Investigating coverage for Student’s t intervals

In this question we shall assume that we have access to a sample X1,…,Xn ∼ N(μ0,σ02) consisting of i.i.d. Gaussain data. We are interested in determining the value of the unknown population mean μ0 based upon the sample X1,…,Xn.

Suppose we wish to compute confidence intervals for μ0 with confidence level (1−α)×100%, for some α ∈ (0,1). For example, we could have α = 0.05, in which cases we wish to compute confidence intervals with confidence

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>library(PairedData)
data("Barley")
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
level 95%. Let X := 1 􏰖n Xi be the sample mean and S := 􏰙 1 􏰖n

n i=1 n−1 i=1

</div>
</div>
<div class="layoutArea">
<div class="column">
(Xi −X)2 be the sample standard deviation. In addition, let tα/2,n−1 be the (1 − α2 )-quantile of the Student’s t-distribution with n − 1 degrees of

</div>
</div>
<div class="layoutArea">
<div class="column">
freedom.

The Student’s t confidence interval for μ0 is given by (L(X1, . . . , Xn), U(X1, . . . , Xn)) defined by

tα/2,n−1 Lα(X1,…,Xn):=X− √n ·S

tα/2,n−1 Uα(X1,…,Xn):=X+ √n ·S.

The following code generates a function student_t_confidence_interval, which takes as input a sam- ple X1 , . . . , Xn given as a vector along with a confidence level γ = 1 − α and outputs a tuple containing Lα(X1,…,Xn) and Uα(X1,…,Xn):

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
student_t_confidence_interval&lt;-function(sample,confidence_level){

sample&lt;-sample[!is.na(sample)] # remove any missing values n&lt;-length(sample) # compute sample size mu_est&lt;-mean(sample) # compute sample mean sig_est&lt;-sd(sample) # compute sample sd

alpha = 1-confidence_level # alpha from gamma t&lt;-qt(1-alpha/2,df=n-1) # get student t quantile l=mu_est-(t/sqrt(n))*sig_est # lower u=mu_est+(t/sqrt(n))*sig_est # upper

<pre>  return(c(l,u))
  }
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Check that you understand this function and implement it for yourself.

The key property of a confidence interval for μ0 at the confidence level of (1−α)×100% is the following coverage property:

P{Lα(X1,…,Xn)≤μ0 ≤Uα(X1,…,Xn)}≥1−α.

This is known as a coverage property since it tells us that the confidence interval covers μ0 with probability 1−α.

The following simulation checks this property with μ0 = 1, σ0 = 3 and a confidence level of 95% i.e. γ = 0.95.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>num_trials&lt;-100000
sample_size&lt;-30
mu_0&lt;-1
sigma_0&lt;-3
alpha&lt;-0.05
</pre>
set.seed(0) # set random seed for reproducibility

single_alpha_coverage_simulation_df&lt;-data.frame(trial=seq(num_trials))%&gt;% mutate(sample=map(.x=trial,.f=~rnorm(n=sample_size,mean=mu_0,sd=sigma_0)))%&gt;%

# generate random Gaussian samples mutate(ci_interval=map(.x=sample,.f=~student_t_confidence_interval(.x,1-alpha)))%&gt;% # generate confidence intervals

mutate(cover=map_lgl(.x=ci_interval,

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
.f=~((min(.x)&lt;=mu_0)&amp;(max(.x)&gt;=mu_0))))%&gt;% # check if interval covers mu_0

<pre>  mutate(ci_length=map_dbl(.x=ci_interval,
                       .f=~(max(.x)-min(.x))))
</pre>
<pre>  # compute interval length
</pre>
single_alpha_coverage_simulation_df%&gt;% pull(cover)%&gt;%

mean() # estimate of coverage probability

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>## [1] 0.95003
</pre>
Check that you understand the above code. Now modify the above code to conduct a simulation experiment to investigate how P{Lα(X1,…,Xn)≤μ0 ≤Uα(X1,…,Xn)} varies as a function of the confidence level γ = 1 − α.

How does the average length E(|Uα(X1, . . . , Xn) − Uα(X1, . . . , Xn)|) vary as a function of the confidence level γ = 1 − α?

6 (Optional) Wilson’s confidence interval for proportions

The following code uses Wilson’s method to compute 99%-level confidence intervals for the pass rate of a driving test.

<pre>library(PropCIs)
</pre>
Use Wilson’s method to compute a 95%-level confidence interval for the proportion of red-tailed hawks who weigh more than a kilogram.

7 (Optional) The Binomial test

The “Airlines” data set contains arrival records for LaGuardia and O’Haire airport. We can load the “Airlines” test as follows:

Extract a subset of the data set corresponding to arrivals of flights with the Delta airline at the O’Hare airport.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
driving_test_results&lt;-c(1,0,1,0,0,0,0,0,0,1,0,0,0,1,0,1,0,1,0,1,0,0,1,0) alpha&lt;-0.01 # failure probability

num_successes&lt;- sum(driving_test_results) # total passes sample_size&lt;-length(driving_test_results)

scoreci(x=num_successes, n=sample_size, conf.level=1-alpha) # compute Wilson’s confidence intervals

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>library(Stat2Data)
data("Airlines")
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
Carry out a statistical hypothesis test to test the hypothesis that 87.5% of the arrivals of flights with the Delta airline at the O’Hare airport are on time. Use a significance level of 0.05. You can use the binom.test() function. What assumptions are required for this hypothesis test?

8 (Optional) Bootstrap confidence intervals

The following code computes a 95%-level confidence interval for the mean weight of the penguins.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
library(boot) # load the library set.seed(123) # set random seed

<pre>#first define a function which computes the mean of a column of interest
</pre>
compute_mean&lt;-function(df,indicies,col_name){ sub_sample&lt;-df%&gt;%slice(indicies)%&gt;%pull(all_of(col_name)) # extract subsample

return(mean(sub_sample,na.rm=1))}# return median

# use the boot function to generate the bootstrap statistics

<pre>results&lt;-boot(data = penguins,statistic =compute_mean,col_name="body_mass_g",R = 1000)
</pre>
<pre># compute the 95%-level confidence interval for the mean
</pre>
<pre>boot.ci(boot.out = results, type = "basic",conf=0.95)
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Explain the importance of the random seed. What assumptions underpin this method?

Compute a 99%-level confidence interval for the median weight of the hawks using the Hawks data set. What can we say about the relationship between the average Hawk weight and the average penguin weight?

9 (Optional) Investigating the failure probability for Wilson’s method

This problem is a more challenging optional extra. Conduct a simulation study based on Bernoulli samples

X1, · · · , Xn ∼ B(q) with n = 100 and q = 0.5. Wilson’s method generates a pair [Lˆn,α(X1, · · · , Xn), Uˆn,α(X1, · · · , Xn)] so that for a given failure probability α, we have

􏰗ˆ ˆ 􏰘

P Ln,α(X1,···,Xn)≤q≤Un,α(X1,···,Xn) ≈1−α.

This approximation is based on the central limit theorem. Conduct a simulation study to investigate how the probability P[Lˆn,α(X1, · · · , Xn) ≤ q ≤ Uˆn,α(X1, · · · , Xn)] depends upon α.

10 (Optional) Effect size for the one sample t-test

In this question we introduce a natural measure of effect size for the one sample t-test considered in question 2. Suppose we have a sample X1, · · · , Xn. We assume that X1, · · · , Xn ∼ N (μ, σ2) are sampled independently and identically distributed from a Gaussian distribution. Our null hypothesis is μ = μ0 and our alternative is μ ̸= μ0 for some μ0 ∈ R. Suppose that our p-value is sufficiently small that we are justified in rejecting the null.

</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
We conclude that μ ̸= μ0. The Cohen’s d-statistic for the one sample t-test is computed as follows: dˆ = X − μ 0 ,

SX whereX=1􏰖n XiandSX=􏰙1 􏰖n 􏰅Xi−X􏰆2.

Create a function called “effect_size_one_sample_t_test” which computes Cohen’s d statistic for the one sample t-test. The function should have two arguments: The first input is a vector x corresponding to the sample X1, · · · , Xn. The second “mu” corresponds to the quantity μ0 in the null hypothesis.

In question 2 we carried out a one sample t-test do test the hypothesis that the population mean of the Adelie penguin’s bill lengths is 40mm. We rejected the null at a significance level of 0.01. Apply your function “ef- fect_size_one_sample_t_test” to compute the effect size. Comment on the magnitude of the effect.

11 (Optional) Confidence intervals for the exponential distribution

Suppose that X1,…,Xn ∼ fλ0 are independent and identically distributed random variables with exponential distribution and probability density function

􏰕λ0e−λ0x if x ≥ 0 fλ0(x)= 0 ifx&lt;0.

Given α ∈ [0, 1] let zα/2 be the (1 − α/2)-quantile of a standard Gaussian random variable Z ∼ N (0, 1). We can compute an (approximate) confidence interval with a confidence level of (1 − α) × 100% for λ0 as follows:

1􏰇 zα/2􏰈 Lα(X1,…,Xn):=X 1−√n

1􏰇 zα/2􏰈 Uα(X1,…,Xn):=X 1+√n .

Create a function which takes as inputs a vector called sample consisting of i.i.d. exponentially distributed random variables X1 , . . . , Xn ∼ fλ0 , and a confidence level confidence_level (γ = 1 − α) and outputs a confidence interval(Lα(X1,…,Xn),Lα(X1,…,Xn))fortheparameterλ0 withconfidencelevelγ=1−α.

Next conduct a simulation study to explore P (Lα(X1, . . . , Xn) ≤ λ0 ≤ Uα(X1, . . . , Xn)) as a function of the confidence level γ = 1 − α.

Recall that population mean E(X) = 1 and population variance Var(X) = 1 . Use the central limit theorem λ0 λ20

to show that

P(Lα(X1,…,Xn)≤λ0 ≤Uα(X1,…,Xn))≈1−α, when the sample size n is very large.

</div>
</div>
<div class="layoutArea">
<div class="column">
n i=1 n−1 i=1

</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
