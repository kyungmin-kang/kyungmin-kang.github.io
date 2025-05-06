---
layout: post
title: "What is Data"
date: 2025-05-06
excerpt: "How Everday Information Fuels Data Science."
tags: [Data]
---

You probably don’t think about it, but you interact with data constantly. When you track your steps on a smartwatch, click a product on Amazon, or listen to a personalized playlist—you're not just using an app. You're generating data.

So before we can understand data science, we have to understand what this “data” really is—and how it’s stored, structured, and transformed into insight.

---

## What Is Data?

> **Data** (n): factual information (such as measurements or statistics) used as a basis for reasoning, discussion, or calculation. — *Merriam-Webster Dictionary*

In plain terms, data is anything that captures something about the world or about us—-numbers, words, images, clicks, sounds. It’s the raw material for discovering patterns, making predictions, and improving decisions.

Here are some everyday examples:

- **Healthcare**: A doctor uses your lab results, past records, and symptoms (data) to make a diagnosis.
- **E-commerce**: A store tracks your browsing history to suggest what you might want next.
- **Finance**: An investor watches price movements and earnings data to decide whether to buy or sell.
- **Social Media**: Your likes and shares train the algorithm to show you more of what it thinks you'll engage with.
- **Smart Devices**: Your thermostat learns your habits to adjust room temperature more efficiently.

---

## Organizing Data: Observations and Variables

To analyze data, we first need to give it structure. That usually means organizing it into:

- **Observations** (a row): A thing we’re measuring—-like a customer, product, or transaction.
- **Variables** (a column): A feature or detail we record about each observation—like age, price, or category.

Think of a simple example: a list of students and their test scores. Each student is an observation, and their names, ages, and scores are variables.

---

## Structured Data: Tables, Rows, and Columns

Perhaps the most common way to store data is in a **tabular format**--stored in spreadsheets, Pandas dataframes, CSV files, SQL tables. These data are known as **structured data**. It looks like this:

| Item         | Date       | Number of Items Sold | Price per Unit | Offline Only | Rating |
| ------------ | ---------- | -------------------- | -------------- | ------------ | ------ |
| T-shirt      | 2025-01-10 | 20                   | 15.99          | No           | A      |
| Coffee Mug   | 2025-01-10 | 5                    | 9.50           | Yes          | B      |
| Laptop Stand | 2025-01-10 | 12                   | 22.00          | No           | A      |
| Book         | 2025-01-11 | 3                    | 12.75          | Yes          | C      |
| Sticker Pack | 2025-01-11 | 18                   | 3.99           | Yes          | B      |

Variables here include both **numeric** (e.g. price) and **categorical** (e.g. rating) types. That distinction matters later when we decide what kind of models or visualizations to use. Below are how variables in our example fit into the common classifications of data types:\

**String Data**
- *Item*: Text (string) variable, containing product names in text format.

**Numeric Data**
- *Number of Items Sold*: Numerical (integer) variable, storing the count of how many items were sold.
- *Price Per Unit*: Numerical (float) variable, holding a price value that can include decimals.

**Categorical Data**
- *Offline Only*: Categorical (binary) variable, indicating two distinct categories.
- *Rating*: Ordered categorical variable, where ratings "A", "B", "C" have a natural order yet are not numeric.

---


## Semi-Structured Data: Still Organized, Just Not Tabular

Some data has structure but doesn’t come in neat rows and columns. A common example is a **JSON file** that logs an online order:

```
{
  "order_id": 12345,
  "customer": {
    "name": "Alice Johnson",
    "email": "alice@example.com"
  },
  "items": [
    {"product": "Laptop", "price": 1199.99, "quantity": 1},
    {"product": "Mouse", "price": 25.49, "quantity": 2}
  ],
  "order_date": "2025-02-01",
  "shipped": false
}
```

<!-- THIS IS NECESSARY -->


We can conver this into structured data by flattening in into rows:

| Order ID | Name | Email | Product | Price | Quantity | Date | Shipped | 
|---|---|---|---|---|---|---|---|
| 12345 | Alice Johnson | alice@example.com | Laptop | 1199.99 | 1 | 2025-02-01 | No |
| 12345 | Alice Johnson | alice@example.com | Mouse | 25.49 | 2 | 2025-02-01 | No |


## Beyond Structured Data: Unstructured Data

Let's consider your favorite YouTube video clip. This is full of data--speeches, audio, visuals, etc--but if we think about storing it in a tabular format, it would be rather difficult. Roughly, we can think of these as **unstructured data**:
- Text: Tweets, reviews, transcripts
- Images: Photos, scanned documents
- Audio/Video: Recordings, call logs
This data doesn’t come with clean rows and columns. An important point to remember--structured data refers to the way information is stored and organized, rather than the specific content it holds. That is, if we transform unstructured data into a **tabular format**,  the data then becomes a *structured data*!

### Example: Converting Image Data to Structured Format
The MNIST dataset, used in machine learning, contains thousands of handwritten digit images. Each image can be translated into a table of **pixel intensity values**-—where each pixel becomes a variable.

<!-- ![MNIST DATA](/assets/blog/ARTWORK/mnist_digit_visualization.jpeg) -->
<img src="/assets/blog/ARTWORK/mnist_digit_visualization.jpeg" alt="description" class="blog-inline-img">


| Digit   | ... |  px31 | px32  | px33  | px34  | px35  | px36  | px37  | px38  | px39  | px310 | ... | 
|----|----|----|----|----|----|----|----|----|----|----|----|---|
| 5  | ... | 0  | 0  | 0  | 36 | 170 | 253 | 225 | 242 | 0  | 0 | ... |


This is what allows a model to learn what a “5” looks like—even without being explicitly told.

### Example: Converting Text to Numbers
Let’s say a chatbot reads the phrase:
**"Hello, there."**
We can turn that into structured data by counting word frequency:

| Word | Count |
|---|---|
| Hello | 1 |
| there | 1 |

## Why This Matters

Understanding how data is structured helps you:

- Choose the right tools for storage (spreadsheets vs. databases vs. NoSQL).
- Pick the right methods for cleaning and analysis.
- Know what kinds of questions you can ask and what kind of answers are realistic.

Remember that **data doesn’t have to be numerical** to be useful. Text, images, even clicks and swipes—-all of these can be turned into structured formats we can analyze.

In our next post, we’ll talk about what **science** really is, so that we can finally talk about what **data science** is. We'll learn how the scientific method works, and how it helps us turn raw data into real knowledge.

