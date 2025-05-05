# Alexa Voice Assistant Skill Privacy Transparency

## Project Description

This project evaluates how voice-assistant skills disclose the data they collect by comparing skill descriptions with vendor-level privacy policies, computing privacy-risk scores, and categorizing skills by risk level.

## key findings

* discrepancies between skill descriptions and privacy policies reveal limited transparency in data collection practices
* only 38 percent of skills reference a recognized privacy standard (for example, GDPR, CCPA, HIPAA)


## methodology

1. data collection

   * scrape skill descriptions and vendor-level privacy policies
2. transparency comparison

   * flag mismatches where descriptions and policies differ on data collection details
3. risk scoring

   * compute weighted scores using factors: data sensitivity, unnecessary fields, missing descriptions, review count, ratings
4. categorization

   * assign risk levels: low (≤4), medium (5–8), high (>8)

## risk scoring details

* sensitivity: 2 points per sensitive category
* unnecessary fields: 0.5 points each
* missing descriptions: 1 point
* high review count: 1 point
* high ratings: 1 point

## risk categories

* low risk: score ≤ 4
* medium risk: score between 5 and 8
* high risk: score > 8

## future work

* develop automated auditing tools to flag discrepancies in real time
* extend analysis across multiple voice-assistant platforms for broader insights
* conduct user studies to measure how transparency affects trust and adoption
* propose standardized privacy labels at the skill level to improve compliance
