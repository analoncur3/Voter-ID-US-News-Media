# Voter-ID-US-News-Media

This is a repository that contains scripts used to download US News Media data.

## Data
-	**Sources**:

| Right       | Left        |
| ----------- | ----------- |
| Fox News      | Washington Post       |
| Washington Examiner   | New York Times        |
| Washington Times   | MNSBC        |
| New York Post   | CNN        |
| Breitbart   | NBC News        |
| Wall Street Journal   | USA Today      |
| Daily Caller   | Vox      |
| Free Beacon   | Chicago Tribune      |
| National Review   | Huffpost     |


-	**Timeframe**: 01/01/2013 - 30/01/2022
-	**Key terms**: "voter ID" or "voter identification" or "ID law" or "ID laws" or "voting ID"


## Rationale
- **Sources**: Traditional media still possess great power in setting the agenda (Langer and Gruber 2021). Mass media plays an important role in legitimizing, amplifying, and spreading disinformation of topics such as climate change (Merkley and Stecula, 2021), the COVID-19 vaccine (Introne et al., 2020) and election-related conspiracism (Benkler et al., 2020). The selection of news media sources is based on Faris et al. (2017) and Benkler et al. (2020) studies. 
    - Faris et al. develop a media partisanship scale from behavior of partisan Twitter users during the 2016 US election, i.e. media source sharing patterns of those who retweeted Trump or Clinton. To test the robustness of their findings, they expand the inquiry to the partisan proclivities of the supporters of other GOP candidates and the supporters of Bernie Sanders, finding the two scores to be highly correlated (ρ = 0.97).
    - Benkler et al. study the disinformation campaign that led to widespread acceptance of false voter fraud beliefs and to its partisan distribution pattern. Contrary to the focus of most contemporary work on disinformation, their findings suggest that this highly effective disinformation campaign was an elite-driven, mass-media led process, with social media playing only a secondary and supportive role. study on election related conspiracies in 2020 echoes . They analyse over 55,000 online media stories, 5 million tweets, and 75,000 on public Facebook pages garnering millions of engagements. The findings are consistent with their findings about the American political media ecosystem from 2015-2018, published in [Network Propaganda](https://oxford.universitypressscholarship.com/view/10.1093/oso/9780190923624.001.0001/oso-9780190923624), and Faris et al. media partisanship scores.
    - Media partisanship was further validated via [The Allsides Bias Ratings page](https://www.allsides.com/media-bias/ratings?field_featured_bias_rating_value=1&field_news_source_type_tid%5B%5D=2&field_news_bias_nid_1%5B3%5D=3&title=). 

We select mass-market/top news media identified in these studies.

<p align="center">
  <img src="https://user-images.githubusercontent.com/89010445/163542980-f2f8542f-29bc-4593-aa02-14e007fe9e57.png" alt="Sublime's custom image"/, style="width:800px;">
</p>

- **Timeframe**: The rate at which states successfully passed voter ID laws increased substantially following the 2013 Supreme Court case Shelby County v. Holder. In 2013, the preclearance required by states with a history of racial discrimination (section 5 of the Voting Rights Act of 1965) was deamed unconstitutional, which allowed these states to enact voting laws without first getting approval by the Justice Department or a Federal Court. This ruling opened the gates for states, specially those formerly needing federal preclearance, to change their election laws. The screenshot fron NexisUni below shows a similar rapid increase of news media stories about voter ID from 2013.

<p align="center">
  <img src="https://user-images.githubusercontent.com/89010445/163543724-0a3c62e1-d50f-4366-a4f5-aa9acdd695df.png" alt="Sublime's custom image"/, style="width:200px;">
</p>

- **Key terms**: To find appropriate search terms, I used Mediacloud's ‘Explorer’ option to instantly analyse how digital news media covers voter fraud and voter suppression, the two partisan frames identified in the literature. I selected coverage during the 2016 US Presidential campaign period (August 1, 2016 – January 1, 2017), in U.S. Top Online News 2017 (Top 32 news websites of the year by August 2017 in the United States, according to data from comScore, Activate and Alexa) and cross-checked identical words in the top 10 words associated to each query. The presence of ‘voter ID’ and ‘ID’ as top terms in both the search terms “voter fraud” and “voter suppression” suggests using voter ID (and variations of it) as a key search term could be a good approach to identify frames.


## Strategy:
- We collect urls via MediaCloud API and extract article data using NewsPlease[P]

