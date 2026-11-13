# Who Feels Threatened by AI?

A class project by Team B04: Steven Nguyen, Ilya Barymov, YC Hsu, and Muhammad Rafi.

## What is this project?

We wanted to know which software developers feel that AI is a threat to their jobs.

Our guess was that it depends on where a developer lives. So we asked two questions:

1. Do developers in richer countries feel differently about AI than developers in poorer countries?
2. Do developers in countries with more internet access feel differently than those with less?

## What did we find?

**Developers in poorer countries use AI the most, trust it the most, and worry about it the most.**

| | Poorest countries | Richest countries |
|---|---|---|
| Use AI tools every day | 73% | 47% |
| Trust that AI gives accurate answers | 77% | 34% |
| Say AI is a threat to their job | 18% | 11% |

A few other things stood out:

* **Trusting AI does not make people feel safe.** Developers who trust AI the most are about three times as likely to see it as a job threat as those who trust it the least (36% vs 12%).
* **Internet access matters less than wealth.** Countries with less internet access show the same pattern, but it is weaker and mostly goes away once we compare countries with similar wealth.
* **Some jobs feel it more.** Mobile developers (26%) and front end developers (24%) are the most worried. Embedded developers (10%) are the least.
* **Mid career developers worry most.** Developers aged 45 to 54 report the highest job threat (20%).
* **Newer developers trust AI more.** About 61% of developers with under 5 years of coding trust AI, compared with 33% of those with 30 or more years.

## What data did we use?

* **Stack Overflow Developer Survey (2025):** a large yearly survey where developers answer questions about their work and their views on AI. [Link](https://github.com/StackExchange/Survey/tree/main/packages/archive)
* **World Bank GDP per capita (2025):** a measure of how wealthy each country is. [Link](https://data.worldbank.org/indicator/NY.GDP.PCAP.CD)
* **World Bank internet usage (2024):** the percent of people in each country who use the internet. [Link](https://data.worldbank.org/indicator/IT.NET.USER.ZS)

After cleaning, we had answers from **22,753 professional developers in 65 countries**.

## How did we do it?

1. Cleaned the survey so it only included professional developers with complete answers.
2. Matched each developer to their country's wealth and internet usage.
3. Kept only countries with at least 30 developers, so the percentages are reliable.
4. Compared countries by sorting them into groups, from poorest to richest and from least to most connected.
5. Double checked our results by having an AI model score each developer's trust and worry on a scale of 1 to 10.

## What is in this repo?

| File | What it is |
|---|---|
| `B04_Project_Who_Feels_Threatened_by_AI_.ipynb` | The notebook with all of our code, charts, and explanations |
| `B04 AI Threat Perception Deck (2) (2).pptx` | Our presentation slides |

## How to run the notebook

The notebook was made in Google Colab. Our data is stored in a private Google Cloud folder, so it will only run as is for people we have given access to.

To run it yourself, download the three datasets from the links above and change the file paths in Section 3 of the notebook to point to your copies.

## What to keep in mind

* **This shows a pattern, not a cause.** We cannot say that being in a poorer country makes developers worry about AI. Something else could explain it.
* **The results describe countries, not individual people.**
* **The survey is not a perfect sample.** People who answer a Stack Overflow survey may not represent all developers, and we only had enough answers from 65 countries.

## What should people do with this?

* **Employers:** when you roll out AI tools, also offer training and talk openly about job security. Start with the groups that worry most.
* **AI companies:** be clear about what your tools can and cannot do. Trust alone does not make developers feel secure.
* **Policymakers:** focus training and job support on lower income countries, where AI use and worry are both highest.

## Use of AI

We used Claude to help with debugging, chart design, and proofreading. We used an OpenAI model to create the trust and worry scores. The team reviewed everything. Full details are in Section 12 of the notebook.
