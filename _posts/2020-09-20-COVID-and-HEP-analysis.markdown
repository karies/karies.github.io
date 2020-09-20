---
title: "COVID-19 and High Energy Physics Data Analysis"
layout: post
date: 2020-09-20
image: /assets/images/COVID19-virus.jpg
headerImage: false
tag:
- COVID-19
- "data analysis"
- science
category: blog
author: Axel
description: Interdisciplinary limits
---

### Jump to [tl;dr](#tldr)

---

## High Energy Physics Versus COVID Data Analysis

In HEP, physicists commonly analyze tens or hundreds of gigabytes in the final step of an analysis;
i.e. a fair fraction of a disk drive.
HEP experiments are basically counting experiments, checking how often something happens.
As such, that data consists of large numbers of similar measurements.
Our analysis software (e.g. [ROOT](https://root.cern)) is thus optimized to scanning through massive amounts of data following the same layout again and again, similar to rows in an Excel table, only way more complex.

Physicists are generally experts at statistics; our tools are excellent at analyzing massive amounts of data - so *obviously* we can help with COVID-19? Not really.

### Data Volume

First of all, COVID-19 data is not actually *massive*.
It still fits into Excel; [Our World In Data](https://github.com/owid/covid-19-data/tree/master/public/data) provides the current numbers as a < 10MB text file (as of today).
That's *nothing*.
HEP data analysis uses a specific format for that "similar pattern, a gazillion times" layout of HEP data.
It's both overkill and just not necessary for COVID-19 data.
It's like getting a Catarpillar to plant a flower: could be done, but sounds like waaay too much effort for what you want to achieve.

### Statistics

High energy physicists know how to count, and what the uncertainties are.
The latter part is the real art and science.
For that, we understand every little ingredient of our data taking:

- which fraction of collisions we measure, and the uncertainty on that;
- how well we identify particples, and the uncertainty on that;
- what we should expect to see - yes, and the uncertainty on that.

All of the above numbers are themselves combinations of several measurements or predictions, each with uncertainties.

COVID-19 data is *very* different from that:

- it's medical data;
- it's collected by humans;
- it's location-dependent, geographical data;
- it's time-series data.

#### Medical Data

Unlike our particles, humans are way too complex to just count: they have a medical history, and "healthy or not" isn't really a binary question.
Yes, there's fuzzy quantum states in HEP, too - but those are still super precise and measureable!

Medical data is thus fundamentally different from physics data.
Their precision is often unknown, even for simple measurements like blood pressure, let alone for compound measurements like "you are infected by SARS-CoV-2".
"Infected by one virus? 1000? 1 million? What's the threshold" would be a typical question a physicist might ask.
And I guess a physician might answer: "whatever, the person has fever among other symptoms!"

#### Collected by Humans

Physicists use objective, neutral deivices to measure.
They are imprecise - but we know their precision.
They can be biased, measuring some particles better than others - but we can measure their bias.

Humans measuring aren't just reading off a thermometer:
they need to apply judgement.
Is 37.6 degree Celsius a temperature high enough to count as another COVID-19 symptom?
Even worse, relying on the subject you need to "measure":
diagnosis of anosmia (lack of ability to smell) relies on self-assessment.
And how do you quantify "really not much", "totally"?
Statistics needs numbers, but much of humans' output is based on categorization, because we are not a measurement apparatus.

In summary, data collected by humans is imprecise, and worse with unknown uncertainties, and generally not generalizable throughout the world, across different ages, etc.
Medical data is not like physics data.

#### Location-dependent, Geographical Data, Time-series Data

Physics rules.
(Totally. Well, its rules rule.)
And independently of where you are.
We're not used to analyzing something that's location dependent.
Sure, we can *learn* how to do that, but we generally don't.

When we count, what happens is completely independent of a previous run of the experiment.
What we see is also not influencing any subsequent repetition of the experiment.
We call this "statistically independent".

COVID-19 data is again not like that, at all:
the risk to get infected depends on what happened before; most of the COVID-19 plots have some notion of "time" on the horizontal axis.
It's called "time series data".
And that's not high energy physics style data.
Again - we can learn, and some of our tools are applicable here, too.



## Summary

High enerrgy physicists are data experts of a different domain than what COVID-19 data needs.
We can learn, we can discuss with COVID-19 experts - but the relevance of physicists "analyzing" COVID-19 data is questionable.
Our data is too different, we, the physicists, understand too little from the intricacies of that data.
We physicists would likely not appreciate a Higgs study by a gastroenterologist without that medical person having *some* background in high energy physics.

Let's be realistic and let's not claim the inverse:
we can talk to you about COVID-19 data analysis over a beer or orange juice, but don't trust [our analyses](https://arxiv.org/search/advanced?advanced=&terms-0-operator=AND&terms-0-term=COVID-19&terms-0-field=title&terms-1-operator=OR&terms-1-term=SARS-CoV-2&terms-1-field=abstract&terms-3-operator=OR&terms-3-term=COVID-19&terms-3-field=abstract&terms-4-operator=OR&terms-4-term=SARS-CoV-2&terms-4-field=title&terms-5-operator=OR&terms-5-term=coronavirus&terms-5-field=title&terms-6-operator=OR&terms-6-term=coronavirus&terms-6-field=abstract&classification-physics=y&classification-physics_archives=all&classification-include_cross_list=exclude&date-filter_by=all_dates&date-year=&date-from_date=&date-to_date=&date-date_type=submitted_date&abstracts=show&size=200&order=-announced_date_first) - they are not done by experts of the right field.

---

## tl;dr

With experimental physics data and COVID-19 data being fundamentally different, physicists' expertise cannot be mapped 1:1 onto COVID-19 data.
Physicists' results on COVIDD-19 data are thus not to be trusted, unless the analysis has been peer-reviewed by actual COVID-19 experts, be it virologists or physicians, depending on the study at hand.
