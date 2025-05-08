---
layout: post
title: "What Is Data Science?"
date: 2025-05-05
excerpt: "The Intersection of Data, Science, and Decision-Making"
tags: [Data, Science, Data Science]
---

Now that we’ve explored what data is and how the scientific method works, we can finally bring the two together. **Data science** is where they meet.


---

## A Simple Definition

At it's core, data science is the **practice of using data to generate insight, make predictions, and guide decisions**—all through systematic analysis.

Just as scientists test hypotheses through observation and experimentation, data scientists explore patterns, run models, and refine their understanding using data.

---

## A Few Real-World Examples

- A student group A/B tests two flyer designs to see which gets more event signups.
- A company uses purchase history to recommend products you’re likely to buy.
- Netflix experiments with homepage layouts to increase viewer engagement.
- A policymaker analyzes job training programs to see which ones boost earnings.

In each case, data science brings a structured, iterative, evidence-based mindset to solving practical problems.

---

## What Makes Data Science Unique?

Data science draws from many fields, but four stand out as foundational pillars:

### 1. **Statistics & Inference**

Statistics provides the theoretical backbone of data science. Given the long history of statistics, many foundational theories in the field were developed at a time when collecting data was expensive and time-consuming.  The central question here was: given that obtaining data is costly, we have to rely on limited amount of data (called **sample**). What is the best way to get our sample and what can we learn about the real world using the data that we have? So using *sample* and  **hypothesis testing** to draw inference about larger population of interest from a small set of data is at the core of statistics that sets statistics apart from the other disciplines.

> Classic question: Given limited data, what can we reliably say about the whole thing (population)?

### 2. **Computer Science & Optimization**

As data grew larger and models more complex, computer science brought tools to process it efficiently. This includes algorithms, databases, and scalable computation.

Further, as more and more data could be used in analysis as obtaining data becomes less costly and computing power has increased, computer science expanded the field of data science to situations where inference was not needed. Now, we could use data from almost all of the population and situations where theoretical calculation was too complicated.

> Classic question: How do we process large amount of data for meaningful prediction?

### 3. **Economics & Causal Inference**

- Do males earn more than females?
- Does going to college cause increase in lifecycle earnings?
- Does higher IQ cause higher lifecycle earnings?
- Does lowering interest rate increase investment?
- Is Unemployment Insurance program effective?

Economists often deal with questions that have real-life consequences but cannot be directly tested because they are impossible or unethical. For this reason, economists specialize in understanding **causal relationships** from non-experimental (**observational**) data. This means designing clever strategies to separate “what causes what” from mere correlations. 

For example, one question that's been intriguing economists is the question: "Does college education increase one's earnings in the US?" One may say, given that the median earnings of those with a bachelor's degree (\$66,600) is higher than that of high school graduates (\$41,800), the data suggests that the answer is yes. [NCES]\([https://nces.ed.gov/programs/coe/indicator/cba/annual-earnings](https://nces.ed.gov/programs/coe/indicator/cba/annual-earnings)) But this is just correlation, because the characteristics of people who only get high school degree and those who get a bachelor's degree are likely to be different. And because people will make optimal decisions for themselves, people who get college degrees do so because they know that the returns to college will be high; those who only get high school degree do so because they know that colleges are not that beneficial for them. This line of thinking is called **selection** or **endogeneity** in economics.

> Classic question: How do we recover *causal effect* from observatinonal data?

### 4. **Domain Knowledge & Business Understanding**

No amount of data matters without the right context. Data scientists need to ask the right questions and translate results into practical actions that people care about.

> Classic question: What KPI are we trying to move and why?

---

## A Shared Principle: Loss Minimization

Across fields, one concept shows up again and again: **loss minimization** (and a close companion, **likelihood maximization**).

Every model-—from a linear regression to a deep neural net—-aims to reduce the difference between what it predicts and what actually *happens*. Every predictive model achieve this by minimizing the difference between what model predicts and what actually *happened*. 

This gap between prediction and actual observation is called **loss**, and minimizing it is the foundation of nearly all modeling in data science. Differences in most of the models simply boils down to how we measure the magnitude of the gap. For example, 

- In linear regression, we minimize squared 'vertical' distance. 
- In Principal Component Analysis (PCA), we minimize the 'minimum distance'.
- In LASSO or RIDGE regression, we minimize squared vertical distance with some penalty terms.

Closely tied to this is **optimization**, or finding the best parameters to minimize that loss efficiently and reliably. How to handle optimization routine gave rise to fance methods such as Gradient Descent (GD), Stochastic Gradient Descent (SGD), Batch Gradient Descent, and so on. Just remember for now that all of these are simply methods to find the minimum.

---

## The Data Science Process

Data science isn't just tools—it's a process. Here's a typical workflow, mapped to the scientific method:

1. **Ask a Question** (Observation, Background)
2. **Form a Hypothesis**
3. **Collect & Prepare Data**
4. **Explore & Analyze Data**
5. **Model & Predict**
6. **Communicate Results & Take Action**

Example: A business facing falling profits might…

- Ask: Why are profits declining?
- Hypothesize: It’s due to increased churn or decreased conversions.
- Gather data: revenue, traffic, retention, marketing spend.
- Analyze: Are costs up? Are customers leaving?
- Model: Predict how different scenarios affect profit.
- Act: Propose changes to product, pricing, or strategy.

---

## Who Counts as a Data Scientist?

Throughout this blog (and eventually this book), we take a broad view. You don’t need the title "data scientist" to *be* a data scientist.

- Business analysts who build dashboards and make evidence-based decisions.
- Researchers who analyze trends and test hypotheses.
- Independent thinkers who dig into public data for answers.

The tools may differ—but the mindset is the same.

---

## How the Role Is Changing

As tools become more powerful and Generative AI starts to automate coding, the **value of human insight goes up**.

Modern data scientists are less about writing perfect code (and traditional data scientists are notoriously bad at writing codes from a computer scientists' view), and more about:

- Asking the right questions
- Framing problems so that it can be answered using data
- Thinking critically both about big and small pictures
- Validating AI-generated outputs effectively
- Interpreting results clearly
- Effectively communicating the findings to stakeholders

You don't need to be a good executional of the computations. You do need to be a good story teller, backed by data.

---

## What Do Data Scientists Actually Do?

They solve problems like:

- **Description**: What’s happening?
- **Comparison**: How does A differ from B? or Is A more effective than B?
- **Classification**: Which group does this belong to?
- **Prediction**: What’s likely to happen next?
- **Optimization**: What’s the best way to act?

Example: A company wants to expand into a new region. A data scientist might…

- Describe sales trends (Description)
- Compare similar markets (Comparison)
- Identify customer segments (Classification)
- Predict revenue potential (Prediction)
- Recommend a strategy (Optimization)

---

## Why Learn Data Science?

Because it makes you a better thinker, problem-solver, and communicator.

You’ll learn how to:

- Frame questions precisely
- Gather and analyze evidence
- Challenge assumptions with facts
- Guide decisions with confidence

Whether you’re in business, academia, policy, or something else entirely, data science gives you tools to **think clearly in a noisy world**.

---

Next time, we'll begin our deeper dive into the methods that make data science work--from preparing and cleaning data to modeling. 

Until then, remember that data science is not just about programming or statistics—it is about *making informed decisions and solving real-world challenges.*

