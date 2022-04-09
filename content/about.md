---
title: "About"
author: "Bristol Priebe"
date: "4/8/2022"
output: html_document

---

# Ratings

We have baseball ratings for NCAA Division I, Division II, and Division III from 2012-present and for NAIA from 2018-present. Score data was obtained from http://ncaa.com and from http://masseyratings.com. Initial ratings are derived by using the score and site of each contest with only same-division games considered. The following adjustments were made and tested within each division to find the combination with the best predictive ability over the past nine seasons:

* How long to combine preseason rating with current season rating
  + From 0 to 60 games
* Whether to cap margin of victory
  + Ranging from cap of 1 to no cap
* Value of home field advantage
  + Ranging from 0 to 1 runs to 4 decimal places
* Whether to include ratings from 2-5 seasons prior in preseason rating
  + Multiple linear regression was used to find the best combination of prior year(s) and then tested
  
# Glossary

* SOS (Strength of Schedule)
  + The value for our SOS is based on the expected winning percentage of an average team against that schedule
  + A lower value means a tougher schedule and vice versa
* SOR (Strength of Record)
  + This is a plus or minus value showing how the team has fared against their schedule vs the expected record of an average team
  + A positive value means the team won more often than an average team would have and vice versa
  + This levels the SOS and illustrates which teams have performed best against their schedule regardless of difficulty
  