# Assignment 1: Protests

During the past few years in the United States, there has been a surge of protests in support of the Black Lives Matter movement, women's rights, trans rights, immigration reform, gun control, the environment, and many other social and political issues.

In this assignment, you will work with data from [CountLove](https://countlove.org/), a group that collects data about protests from across the United States, including information about the purpose of the protests, the location of the protests, as well as how many people attended the protests. This data has often been [cited by the *New York Times*](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html), among other major outlets.

Through this assignment, you will be able to answer questions including: - What were the most attended and least attended protests in the US in the last 5 years? - How many protests occurred in Washington state? - How did the number of protests in 2019 compare to 2020, and why? - Why are people protesting in the US? What are the biggest motivators?

This assignment is divided into 2 parts. You will complete your coding work in the `analysis.R` file, and you will write short answer responses related to critical analysis and reflection of the data in this `README.md` file. Before getting started on your coding work, you should complete the section **"Critical Analysis & Reflection: Before You Code"** below.

When you are finished with the assignment, be sure to push all changes to your GitHub repository and then submit the link on Canvas.

## Before You Code: Critical Analysis & Reflection

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out *domain familiarity* --- in other words, knowledge about the subject/topic of the dataset. (We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it.)

To get more familiar, we are going to begin by doing some background reading.

-   First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm). Based on the information in these pieces, why did the creators start collecting the CountLove data? Please answer in 2-3 sentences (3 points)

    **The creators start collecting those data in order to get more comprehensive data to support on protests in the U.S. They try to use those data to capture more patterns, trends and the impact with the protests. Additionally, they try to seek more information for those researchers, journalists, policymakers, and public for more precise decision making.**

-   Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)

    **The article discusses the widespread and powerful impact of the Black Lives Matter movement in America following the death of George Floyd. It highlights the unprecedented scale and diversity of protests across the country, reaching even rural, conservative, and majority white communities. The movement's ability to transcend traditional fault lines and spark conversations about systemic racism and the daily hardships faced by black Americans is seen as a potential catalyst for lasting change.**

Next, we're going to reflect about who collected this data, and what's actually inside it.

-   Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)

    **Nathan, who is a scientist and Tommy, who is a engineers collect those data. Those people who are interesting in the topic sharing the data.**

-   As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)

    **CountLove includes "*count public displays of protest that are not part of \"regular business.\"* , while excluding "*awareness events, commemorative celebrations, historic reenactments, fundraising events, townhalls, or political campaign rallies*".**

-   How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)

    **CountLove obtains a significant portion of their protest data by crawling local newspaper and television sites on a daily basis. These crawls allow them to collect information directly from these sources, ensuring a comprehensive coverage of protests.**

-   How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)

    **CountLove adopts a conservative approach to estimating the attendance numbers by recording the** **most conservative figure mentioned in the news articles they analyze. They interpret vague attendance descriptions, such as "a dozen" as 10 and "dozens" as 20. However, relying solely on news articles for attendance counts can introduce potential problems. It may lead to underestimation if the actual attendance surpasses the conservative figures mentioned in the articles. Additionally, when articles don't provide an attendance count, CountLove leaves the count empty, which could result in incomplete data for some demonstrations.**

## While You Code: Critical Analysis & Reflection

-   Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)

**The basic reason that mean is higher is higher reason is that this data is skewed to the right, which means there are few large attendees that influence the overall average number of attendees.**

-   Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point) \*s Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences

    Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences

**I think there were more protests in 2019 than in 2018, because as the there are more social issue appear between 2018 and 2019, the protest might increase.**

**I think there were more protests in 2020 than in 2019, because the COVID-19 problem arise during that period of time, people are strggule of dealing this issue.**

-   Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)

    **The number of protests from 2018 to 2019 to 2020 does not surprise me, because the data shows the number of protests during the 3 time increase. This might caused by the increase of political issue, public events and so on.**

-   Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)

    **The first most frequent category of protest, "Civil Rights," aligns with the major protest movements in the U.S. in recent years. The country has witnessed significant activism and demonstrations surrounding civil rights issues, such as racial justice, police brutality, and equality. The fourth most frequent category, "Environment," also aligns with the growing awareness and concern for environmental issues, including climate change and sustainability. Both categories reflect the significant social and political movements that have emerged in response to these pressing issues.**

## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action: \> Taking action can itself take many forms, and in this chapter we offer four starting points:\
\> (1) Collect: Compiling counterdata---in the face of missing data or institutional neglect---offers a powerful starting point as we see in the example of the DGEI, or in María Salguero's femicide maps discussed in chapter 1.\
\> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.\
\> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as "fairness," but as co-liberation.\
\> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?

-   How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)

    **The CountLove project embodies the form of challenging power through "creating alternatives" by providing a comprehensive and inclusive database of protests that is distinct from traditional sources of information. By collecting and sharing data on demonstrations that are often overlooked or underrepresented in mainstream media, CountLove challenges the power structures that control the narrative and selectively amplify certain voices. Furthermore, CountLove's emphasis on grassroots activism and community-driven events aligns with the form of challenging power through "engaging directly" with the issues and promoting participatory democracy. The project empowers individuals and communities to have their voices heard and contributes to a more accurate and nuanced understanding of social and political movements.**

-   What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)

    **It is surprising to see that environmental protests, which address critical global issues, rank fourth in frequency. This underscores the significance of activism focused on environmental concerns and the growing awareness of environmental issues among the general public.**

-   What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

**One interesting analysis that could be done with CountLove data is to examine the correlation between protest events and various socio-economic indicators, such as income inequality, unemployment rates, or political affiliations. This analysis could provide insights into the relationship between social unrest and broader societal factors. Additionally, conducting sentiment analysis on news articles related to protests could reveal the overall tone and framing of media coverage, shedding light on media bias and its impact on public perception of protests.**
