---
layout: post
title: "The Early Days of FluidMind and Euthymia Technologies"
author: "Charlie"
categories: blog
tags: [blog,fluidmind]
image: blog1.png
---

<small>10 min read</small>

Have you ever thought to yourself, "am I depressed?" And then you went online and did a simple "Am I Depressed?" quiz, and got a damning result. And then you thought, well, what if I also have OCD? So you went and looked for the OCD quiz, and got your results. "What's the point of all the rigamarole - why don't we just compile it into one test?" That's the thought I had, sitting on my bed one day, unemployed but overly educated, that led to the birth of Euthymia Technologies.

### If I can't find a job, then I'm going to have to make myself a job.

I had recently lost my job, as had many in the software industry, right around the time that Elon Musk started cutting half the staff at Twitter ([now known as X](https://twitter.com/euthymiatech)). This sent a shockwave throughout the tech industry. One-by-one tech companies started laying off their staff in anticipation of the incoming recession. Tech was, and still is, not in good shape, and software engineers are taking the brunt of that shockwave.

I had one year of software experience in industry behind my belt, and various degrees in the computational sciences and applied mathematics, so I thought that "this shouldn't take me too long to find something new." But I was wrong - in a crumbling economy, new jobs in AI are gate-kept from those with little to no experience, like myself.

So I thought "*if I can't find a job, then I'm going to have to make myself a job*."

### But what would that look like?

In between dropping out from graduate school and my first job in tech, I had toyed with the idea of making my own startup. Like many others, I grabbed a copy of "[The Lean Startup](https://www.amazon.ca/Lean-Startup-Innovation-Successful-Businesses/dp/0670921602/ref=asc_df_0670921602/?hvadid=293006252041&hvdev=c&hvdvcmdl&hvlocint&hvlocphy=9000910&hvnetw=g&hvpone&hvpos&hvptwo&hvqmt&hvrand=10443926367184204382&hvtargid=pla-364195445884&linkCode=df0&mcid=27ef50f7b1cc3e8cb7b5bd69ab0f107d&psc=1&tag=googleshopc0c-20)" by Eric Ries and started coming up with viable ideas. I concluded that the future of mental health would be the infusing of machine learning into new technologies used in the clinic.

But what does machine learning require? Data. Lots of data. And what does the mental health field lack? Data. Lots of data. This lack of big data in mental health proved to be the demise of all my ideas that utilized machine learning.

So I thought "*if the data doesn't exist, then I'm going to have to collect the data*."

### What data is worth collecting?

To understand what data is worth collecting, we first have to understand what exactly machine learning does.

There's two main categories of machine learning: unsupervised learning, and supervised learning. In unsupervised learning you cluster data together to find common features - effectively, you want to label the data. In supervised learning, you already have the labels, and you typically want to predict the label of new data points.

Here's an example: let's say I have an image of an animal, and I can identify that animal as a cat, so I label the image "cat". Could I make a machine capable of telling me whether or not a new image (the data point) contains a cat within some degree of accuracy? It turns out, if you have millions of images which are labelled as "cat" or "non-cat", you can train a machine learning model on that data, and hence give it the ability to predict whether or not a new image has a cat in it. That's supervised learning - it's predictive.

### How could you apply machine learning to mental health?

What predictive modelling would be useful for mental health? I can think of two major contenders: 1) predicting an effective medication for a patient, and 2) predicting a diagnosis. What kind of data would we need to do this?

For Point 1, we could imagine making measurements such as a: blood test, brain scan, genetic screening, and EEG. It's possible that this combination of data would provide enough predictive power for a machine learning model to indicate an effective medication for an individual. But in order to train this model, we would need a huge, clinically verified dataset. That costs money to procure - money that I and nonetheless most organizations do not have.

How about Point 2? [Kintsugi](https://www.kintsugihealth.com/), a startup in the Bay Area, hypothesizes that they can predict a person's diagnosis using free-form speech data. That is to say: they make a recording of you speaking, perhaps to a therapist or doctor, and they use that data to make a prediction of whether or not you have, say, major depressive disorder.

### My Idea

I have another idea, which I think is easier.

Ultimately, a diagnosis is made by a psychiatrist through a screening: they ask you a set of questions, they analyze your background and history, they observe your behaviour, they track your progression in life in all domains, and then they say with some certainty, "yes, I think you have major depressive disorder."

A key part of this process is asking you questions. How has your mood been the last two weeks? How about your appetite? Can you describe the content of these thoughts which overcome you? Are there any repetitive behaviours you use in response to these thoughts?

Based off the answers to these questions, they can formulate an idea as to what disorder you might have, and once they have this information, they can pinpoint an effective treatment such as a specific therapy and/or medication. You see, before they can treat the problem, they have to define what that problem is.

Could we make a machine (in this case, a software) that can do this, or at least aid in the process? In order to pull it off, we would need lots of data which connects people's answers (to these various questions) to the disorder they've been diagnosed with.

That process has three components:

* Have many people answer these questions.
* Have doctor's confirm those people's diagnoses.
* Collect and analyze all that data.

### FluidMind

That's when I had the idea. I know, from my own experience, that answering those questions can be fun - even addictive. It's the same with doing a personality test. The questions are interesting, they're fun to think about and to reflect on, and then you get a tangible result that gives you a deeper insight into something you already knew about yourself or better, it shows you something you missed.

So I imagined an app that compiles all these questions into one source, and gives you instant feedback into a range of symptoms and disorders you could have. I thought, "I can build that app." Enter: [FluidMind](https://euthymiatechnologies.com/fluidmind).

I had never built an app before, but I had done plenty of software in grad school. So I taught myself React Native, which required learning React, which required learning JavaScript and HTML. I had never even read code written in these languages, but as it goes in coding, once you master a few languages, you've basically mastered them all. I had experience writing: Python, C/C++, MATLAB, Fortran, and Bash. I followed [Full Stack open](https://fullstackopen.com/en/) to learn React Native, and before you know it I was off to coding FluidMind.

### Trust in FluidMind

FluidMind solves the first component: *Have many people answer these questions*. The next two components are way off in the future, but I will say this: it's going to take a lot of effort to build the trust necessary to convince people to let my company collect their mental health data, even if it's fully anonymized. For now, **<span style="color: #3366ff;">I will not collect that data at all</span>**. FluidMind encrypts all your results and stores them locally to your phone - **<span style="color: #3366ff;">none of it is put on external servers</span>**.

It might even be possible that this day of full trust may never come. But if that's the case, then I hope in the meantime I can build something that people love to use regardless of the reason I started it.

But FluidMind does more than just give you an indication to your potential symptoms and disorders, it will track your scores through time. Over the weeks of using the app on a daily basis, your results will evolve, and you can watch those fluctuations to keep track of your mental health. That's why I put the word *fluid* in FluidMind. Your mental health is not just composed of some rigid symptoms - your symptoms evolve and flow through time.

### So where does the company come into the picture?

Can't you publish an app without a business? Nope! Not if you're going to make money off of it, which I plan to using ads. But then there's also the logistics: the Google Play Store requires that you have a DUNS number (a business identification number), and to get that you need a business. So, I started Euthymia Technologies.

And as I've been working on the app, my vision for the company is growing. I didn't call it "Euthymia Technology", I used the word *Technologies* (plural) because I believe that we can build more than just an app. FluidMind is just the starting point. I imagine a future where Euthymia Technologies makes major contributions to alleviating the suffering that is felt across the world from mental illness. So I've made it the company's mission to make sure **<span style="color: #3366ff;">every person with mental illness experiences at least one euthymia (a period of normal, healthy functioning of the mind) in their lifetime</span>**.

Just as with the app, I thought, "I can build that company."
