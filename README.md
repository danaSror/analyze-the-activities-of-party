# analyze-the-activities-of-party
---
The goal is to analyze the activities of the party and the Knesset member over the past year through social networks or articles.
But despite the attempts, the results seemed less satisfactory because of the "dirty" information structure of tweets. In addition, the tweets are in the Hebrew language and there are not enough models that are well trained in the Hebrew language.
After this attempt, I extracted news correspondence information using the Google API but got minimal information in terms of dates because it is a limited API.
But at the same time, the results seemed satisfactory and logical.
---
**My solution to the problem described is:**

***First attempt:***

1️⃣ Download tweets from Twitter for the last month (API is restricted and does not return results for older dates)

2️⃣ Identify issues using a BertTopic model

3️⃣ Visual presentation in different ways of the identified topics
After realizing that the results were less quality, I switched to the following experiment:

***Second attempt:***

1️⃣ Download articles from Google (limited in the number of repeated results)

2️⃣ Create an orderly DF of the returned results concerning the dates of the articles.

3️⃣ Training the information from the articles using BertTopic model for identifying topics

4️⃣ Present the events identified from the articles visually.
