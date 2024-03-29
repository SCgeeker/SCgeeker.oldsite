---
layout: post
title:  Display Math Equation in Post
date: 2017-04-07
published: true
categories: [statistics, latex]
---

There will be many posts demostrate how to transfer the mathematical laws to the codes, and the reversed flaw. I start from this famous equation:  

$$ E = mc^2 $$   

Use the steps 1 and 2 indtroducted in [Fong Chun Chan's post](http://tinyheero.github.io/2015/12/06/rmd-to-jekyll-protect-eqn.html), my website is able to show the equation in any post. Because this theme use `kramdown` as the engine of markdown, I pass the step 4. 

Here are the proof the central limitation theorem. Mix of inline and one-line equations.  
We have a sequence of independent random variables,$$ X_1, X_2, \ldots $$  
And the mean and variance of them:  
Mean $$ E \left[{X_i}\right] = \mu \in \left({-\infty \,.\,.\, \infty}\right) $$  
Variance $$ V \left({X_i}\right) = \sigma^2 > 0 $$  

Assume:  
$$ S_n = \sum_{i \mathop = 1}^n X_i $$  
Then:  
$$ \displaystyle \frac {S_n - n \mu} {\sqrt {n \sigma^2} } \xrightarrow {D} N \left({0, 1}\right)$$  as  $$ n \to \infty $$  

Embedded tex codes in `$$ ... $$`, the equation was transfered inline or in single line. Thus I pass the step 3 of [Fong Chun Chan's method](http://tinyheero.github.io/2015/12/06/rmd-to-jekyll-protect-eqn.html).

**Note.** Justify the last equation in 2017-04-07 19:31:38
