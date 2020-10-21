---
title: Project Markdown'
author: "Hribal"
date: "9/30/2020"
output: html_document
---

## Analysis of 2020 MLB Season Statistics 

Edward Hribal
edhribal@iu.edu
INFO-I 423

# Abstract

The 2020 Major League Baseball season was abridged due to the COVID-19 pandemic and labor strife interrupting plans to resume play. Due to these factors, the regular season only consisted of 60 games, compared to 162 games in a typical regular season. This sudden change in the length of the season could potentially disrupt player evaluation and projection systems, as a sample size being reduced by nearly 63% could result in a misinterpretation of player ability based on an aberrant performance in a small sample. This season’s statistics need to be analyzed to determine their reliability against a full 162 game season.

Contents

{{< table_of_contents >}}

{{% /pageinfo %}}

# 1. Introduction

TBD

# 2. Datasets

The data I will be using for this analysis comes from the Lahman database, Fangraphs, Baseball Reference, the Chadwick Bureau, Retrosheet, and Baseball Savant. These datasets can be easily utilized in Python by installing 'pybaseball' via pip. At the moment I do not know precisely what data I will be utilizing from each source, but this library contains more than enough data for me to conduct my analyses.

# 3. Preliminary Analysis

One test I wanted to do was determine if certain statistics had the same predictive power that they had in previous years. To start, I assigned a player name and OPS for the years 2018, 2019, and 2020 in different data frames, then calculated the correlation between their OPS in 2018-2019 and 2019-2020. The initial results show that this years statistics were less predictable based on conventional measures than in previous years. The correlation for 2018-2019 was .495, and the correlation for 2019-2020 was .376.

# 4. Next Steps

I want to do this test for the last 25 years of statistics to get the average correlation between different predictive stats, then compare them to this year's correlation to last year. I also want to test if different projection system's predictions for this year were unusually worse compared to previous years. Afterwards, I hope to come to a conclusion on how to normalize these stats so they can be compared more easily to previous and future seasons. I will look into the variability that players have in 60 game intervals as one route for this.