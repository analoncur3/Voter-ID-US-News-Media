# Voter-ID-US-News-Media

This is a repository that contains scripts used to download US News Media data

## Data
-	Sources:

| Right       | Left        |
| ----------- | ----------- |
| Fox News      | Washington Post       |
| USA Today   | New York Times        |
| Washington Times   | MNSBC        |
| New York Post   | CNN        |
| Breitbart   | NBC News        |

-	Timeframe: 01/01/2013 - 30/01/2022
-	Key terms: "voter ID" or "voter identification" or "ID law" or "ID laws" or "voting ID"


## Rationale
Studies have found mass media plays an important role in legitimizing, amplifying, and spreading disinformation of topics such as climate change (Merkley and Stecula, 2021), the COVID-19 vaccine (Introne et al., 2020) and election-related conspiracism (Benkler et al., 2020). The selection of news media sources is based on Faris et al. (2017) and Benkler et al. (2020) studies. Faris et al develops a partisan media scale from media coverage during the 2016 election. Benkler's study on election related conspiracies in 2018 echoes Faris findings around partisanship in media. We select news media that played a key role.

![Faris media scale](https://user-images.githubusercontent.com/89010445/163542153-061cb0b5-543a-477d-bb33-6f68d94c74d8.png)


## Strategy:
- We collect urls via MediaCloud API and extract article data using NewsPlease[P]/Paperboy[R]
- We download data from NexisUni and extract article data using LexisNexisTools[R]

