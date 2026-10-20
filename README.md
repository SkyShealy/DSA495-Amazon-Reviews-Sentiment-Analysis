# Amazon Reviews Sentiment Analysis

> **DSA 495 Topic Brief**
>
> Replace the bracketed prompts below with your team’s information. Keep this file at the root of your team’s project repository and name it `README.md`.

## Before You Begin

- Create **one shared project repository per team** and continue using it through the end of the semester. Do not create separate repositories for the Topic Brief and later stages of the project.
- The repository name must begin with the case-sensitive prefix **`DSA495`**, such as `DSA495-news-classification`. After the prefix, feel free to choose a creative and distinctive team name; it does not have to describe your task or topic. A repository whose name does not begin with `DSA495` will receive zero credit for the Topic Brief.
- Complete every required section and item below. Anything labeled optional may be left undecided! If another required item does not apply, write “Not applicable” and briefly explain why. Feel free to add sections as needed, but keep the brief concise.
- Make sure the repository is accessible to the instructor by choosing one of the following options:
  1. **Public repository:** No collaborator invitation is required.
  2. **Private repository:** Add the instructor as a collaborator using the GitHub username `SerenaYKim`.
- Do not upload sensitive or restricted information to GitHub, even in a private repository. If your project uses such data, keep it in a shared team drive and use GitHub for code, documentation, and other materials that can be shared safely.

## Team Members

- Sky Shealy
- Abigail Ma

## One-Sentence Task

**Given the Amazon ratings in the Video Games category from May 1996 to September 2023, we will analyze the ratings for products in this category and predict the number of stars in future reviews.**

## Illustrative Input and Desired Output

- **Example input:**
| title | review |
|------|-----------|
| Product as described | Perfect! I would recommend |

- **Desired output:**
| Rating Prediction | Confidence Level |
|------------------------|-------------------------|
| 5.0 | 0.988 | 


## Background and Starting Point

Our team is interested in this topic because of our shared interest in video games, and we were both interested in looking at reviews related to video games. These interests inspired us to analyze how consumers view different products in this category, and we ended up finding a dataset containing reviews for video game products from Amazon. 

## Intended Output and Success

We want the project to help predict future reviews and their ratings for different products. Being able to predict future ratings will help determine how well a product does on the market for businesses and companies to see consumers’ views of their product.

**Success statement:** Predicting the number of stars for future reviews will be helpful for determining how future reviewers will rate a specific product. It will also be particularly useful for analyzing how a certain type of product tends to be rated.

## Preferred Data

### Corpus

The collection of text we expect to analyze is the reviews for products located in the Video Games Category in Amazon. One item in the corpus represents a review for a product, which is composed of a star rating, title, and review text. The corpus contains 2.8 million reviews. For our purposes, we have taken a simple random sample of 23,118 reviews. The corpus contains other variables, such as user ID and timestamp, which we have removed to more precisely fit our objective.

### Source and Access

- **Dataset or corpus name:** Amazon Reviews 2023
- **Original source organization or creator:** Hugging Face, Creator: Yupeng Hou (hyp1231)
- **Original collection process:** McAuley Lab (https://cseweb.ucsd.edu/~jmcauley/) collected the data in 2023 from Amazon.
- **Direct link:** https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023
- **Access method:** Download
- **Access, licensing, privacy, or redistribution considerations:** None identified.
- **Backup corpus (optional):** Not needed at this stage.

### Examples

| rating | title | text | 
|------|------|-------|
| 1.0 | dont waste your money | this item makes the games tough to enjoy.get a nintendo brand.cheap is not fun.pay more or you will regret it. |
| 5.0 | Love it | It works great. Load screens load faster than my old xBox One. I'm a fan. I recommend. | 
| 3.0 | Graphics were excellent. | Bought this for my grandkids. They said it was a little disappointing, as it didn't them long to beat the game. Graphics were excellent. |

### Fit with the Task

The corpus is composed of titles and text reviews that are meant to explain the number of stars that a user rated an item as. They should be directly related, which will allow us to predict rating stars given the text content of a review. 

## Feasibility and Immediate Next Steps

- **Minimum viable project:**  A model that predicts the number of stars future ratings will have when given a small sample to analyze.
- **Data-access check:** All team members can access the data and have been able to clean the data for unnecessary variables.
- **Largest current risk:** The most important uncertainty is that the “Video Games” category is quite vague and covers many types of products produced for video games.
- **Backup plan:** If this risk is too large, we can find a different dataset that focuses on reviews for a specific type of video game product or change our focus to a different category that is more centralized on one type of product.
- **Next two actions:**
  1. [Make training and validation splits — Abigail Ma — 11/01]
  2. [Tokenize reviews — Sky Shealy — 11/01]

## Possible Text-Analysis Method and Evaluation (Optional)

[Not yet decided]

## Questions for the Instructor

- Can this project be considered a sentiment analysis?
- Is this more of a regression problem or a classification problem? The review score is ordinal. With classification, the predictions would more accurately reflect the format of the review. With regression, the ordinal nature of the rating scale is preserved more, and MSE could better reflect how well the model is doing than precision and recall, since MSE increases with a greater distance from the observed value unlike precision and recall. Would classification’s cross entropy loss be a more or less appropriate performance metric than regression’s MSE?

## AI-Use Statement

We did not use any AI tools or resources to complete this brief.
