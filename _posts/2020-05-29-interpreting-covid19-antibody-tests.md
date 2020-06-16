---
title: Interpreting COVID-19 antibody test results
date: 2020-05-29
description: What does it mean when a test claims to be "accurate"?
categories:
image: covid_antibody_test.jpg
author_staff_member: michelle
---

COVID-19 <a href="https://en.wikipedia.org/wiki/Serology#Serological_tests" target="_blank" > antibody tests</a> are rapidly becoming widely available.
These are the tests which can tell you whether or not you have previously been infected by the COVID-19 virus SARS-COV-2.
The tests look for <a href="https://en.wikipedia.org/wiki/Antibody" target="_blank"> <b>antibodies</b></a> in the blood which are made by the body in response to infection, and which reach high enough levels to be detectable from about 3 weeks after infection (or 2 weeks after symptoms began, if you had them).
Today in the UK many suppliers have sold out - people are understandably keen to know whether or not they have had the virus.
However, there have been confusing reports in the media about how we can interpret these tests and some have been temporarily withdrawn from sale over questions about their accuracy.
To what extent are these tests useful, and how can we interpret them?

There are two key factors to consider when interpreting an antibody test: what "having antibodies" means for an individual, and how accurate the test is.

## What does "having antibodies" mean?

At the time of writing (29th May 2020) and to the best of my knowledge, there are no clear answers to the questions:
1. Does having antibodies mean you are immune?
2. How long does immunity last?
3. If you have antibodies, can you still be a carrier of the disease?

Until we are sure that having antibodies makes you immune and unable to pass on the disease, and until we know how long that protective effect lasts, it is important that we follow the <a href="https://www.cdc.gov/coronavirus/2019-ncov/testing/serology-overview.html" target="_blank"> <b>offical CDC advice</b></a> which currently cautions against anyone acting any differently on the basis of a positive antibody test.



## What does "accurate" mean?

When I see a test being marketed as "99% accurate" it immediately makes me suspicious.
For tests such as these, accuracy ought to be broken down into two figures: the <a href="https://en.wikipedia.org/wiki/Sensitivity_and_specificity" target="_blank" > <b>sensitivity</b> and <b>specificity</b></a>.
Let me explain.

For a test to be accurate, it needs to correctly tell people who have had it that they have had it (be "sensitive"), and correctly tell people who haven't had it that they haven't had it (be "specific").
After all, I can easily make a 100% sensitive test: it's an envelope, and inside is a piece of paper which says "you have had COVID-19".
I could send one out to everyone in the country, and everyone who has had COVID-19 will get the correct result.
100% sensitive. Bingo! 100% accurate? Obviously not.

I could also make a 100% specific test: it's an envelope containing a piece of paper which says "you have not had COVID-19".
Again, I could send it out to everyone in the country, and everyone who hasn't had COVID-19 will get the correct result.
100% specific. Hurray! You get the idea.

An <b>accurate</b> test has to perform well in both directions; it has to be right most of the time.
But this silly example leads us to an important observation.
In the early stages of an epidemic, and in some countries in the world today, there have been very few cases, and my "you have not had COVID-19" envelope would in fact be right most of the time.
The <b>prevalence</b> of the disease - the proportion of the population who have had it - will affect how often a test gives the right result.
The really counter-intuitive thing is that when prevalence is low, it's extra important that the test has high <b>specificity</b>.
Here's an example to show what I mean.

## An example

To keep the numbers nice, let's consider a place where prevalence is about 10%, so 1 in 10 people have been infected. (In the UK at the end of May 2020 it is probably a bit lower in most areas and a bit higher in some - see <a href="https://www.gov.uk/government/publications/national-covid-19-surveillance-reports/sero-surveillance-of-covid-19" target="_blank"> here</a> for a current report.)
If you test 1000 people (and they are a nice representative sample, etc.) there should be 100 people who have had COVID-19.
If your test is 99% sensitive then 99 of them will get the appropriate positive result; one will not (a "<a href="https://en.wikipedia.org/wiki/False_positives_and_false_negatives" target="_blank" > false negative</a>").
If your test is 98% specific then 882 (= 0.98 x 900) people will get the appropriate negative result.
That leaves 18 (= 900 - 882) incorrectly getting positive results.

Altogether, 117 (= 99 + 18) people get positive results, of whom only 99 have really had it ("true positives").
Therefore, if you are one of those 117 people who get a positive result, there is a <b>84.6%</b> chance you have had it (= 99 / 117 x 100).
That is probably substantially lower "accuracy" than we expected when we first heard that the test was 99% sensitive and 98% specific.

## What can antibody tests tell us?

The interaction of prevalence, sensitivity and specificity is often counter-intuitive and can lead to confusion and sometimes <a href="https://doi.org/10.1080/09540120701867206" target="_blank"> devastating consequences</a>.
The little app below enables you to run the calculation I outlined above for different combinations of values for prevalence, sensitivity and specificity.
Notice how at 1% prevalence (appropriate for many places in the world) a positive result on a 99% sensitive and 99% specific test really only gives you a 50-50 chance of having had COVID-19.
You can check how the <a href="https://www.fda.gov/medical-devices/emergency-situations-medical-devices/eua-authorized-serology-test-performance" target="_blank"> sensitivity and specificity of particular tests</a> available in your area might perform in the context of the local prevalence.

One way to have greater confidence in a test result is to repeat the test.
Testing yourself once a fortnight could help to build a fairly accurate picture of whether or not you have become infected at any point, and may even help to spot waning immunity if and when this happens.
However, with tests currently in short supply and typically costing £60-£150, this is not a practical option for most people.

At a regional or national level, antibody tests can be useful for public health bodies and researchers to build up a picture of how many people have had the virus.
However, the lack of certainty about immunity, together with the lack of clarity about the accuracy of many publicly available tests, make me extremely wary about individuals using them for anything other than casual interest at the moment.


<html>
<head><title>Shiny App Iframe</title></head>
<body>
<iframe id="interpreting_antibody_tests" src="https://mkendall.shinyapps.io/interpreting_covid19_antibody_test_results/?_ga=2.255624129.850956528.1590657787-1388260547.1582025294" style="border: none; width: 100%; height: 1000px" frameborder="0"></iframe>
</body>
</html>
