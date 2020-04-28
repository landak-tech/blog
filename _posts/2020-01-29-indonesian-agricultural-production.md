---
layout: post
title:  "Estimated Indonesian Agricultural Production"
author: joko
categories: [ agriculture, Indonesia ]
tags: [ tableau, KNIME ]
image: assets/images/2.jpg
credit: <a href="https://www.freepik.com/free-photos-vectors/travel">Travel photo created by onlyyouqj - www.freepik.com</a>
description: "This is the description"
featured: true
hidden: true
rating:
beforetoc: "Agriculture is one of the key sectors within the Indonesian Economy, contributing 14.43% of GDP and representing 41% of the country's total labor force, yet it's data availability and consistency for analytics purposes are far from ideal."
toc: true 
---

Few years of experience in the Indonesian agricultural supporting industry, as a decision support system service provider, shows how hard it is to make a decent data-driven decision mainly due to the unavailability of the data. It may be available but restricted for governmental use, so business-oriented organization such ours will find it difficult to exploit the data and find answers for:
- How is the optimum way to source certain agricultural commodities, for a certain quality and price?
- Which regions still have sufficient stock and comply with the required quality?
- How do we prevent fraud within the current trading system?
- and so on. 

## Objectives

Currently, it may be a little difficult to answer advance questions, but otherwise, it may be possible to answer a simpler one. This article is an attempt to predict the estimation of Indonesian agricultural production per year.

## Data Sources

For predictive analytics to succeed, we need to define what kind of data and where are we going to source the data.
1. Indonesian agricultural production data and production (farming) area for each commodity is available from https://bps.go.id, not the central one but the respective regional bodies.
2. Indonesian climate data such as rainfall rate, temperature, humidity, solar radiation, and wind speed are available from https://dataonline.bmkg.go.id.

## Preparation

The above-mentioned data were publicly available in the .csv or .xls format. The data, especially the agricultural-related data, as expected were kind of messy, with missing value, non-uniform format, etc. KNIME Analytics Platform was used to clean, prepare the data, and predicted the outcome. Visualization was made on Tableau Public.

90% of the time was spent to prepare the data. Few KNIME nodes were used for that purpose such as:
- Missing value handling with [Missing Value Node](https://hub.knime.com/knime/extensions/org.knime.features.base/latest/org.knime.base.node.preproc.pmml.missingval.compute.MissingValueHandlerNodeFactory).
- Aggregation with [GroupBy Node](https://hub.knime.com/knime/extensions/org.knime.features.base/latest/org.knime.base.node.preproc.groupby.GroupByNodeFactory).
- Unpivot the already pivoted table with [Unpivot Node](https://hub.knime.com/knime/extensions/org.knime.features.base/latest/org.knime.base.node.preproc.unpivot2.Unpivot2NodeFactory).

We're going to discuss more detail about KNIME another time.

After the data was ready, the data was partitioned so we have a training dataset and testing dataset. Then we analyze the correlation of training dataset related values, built a model to learn from it, predict the production outcome using the testing dataset, and export the data to a .csv format.

## Analysis

<center>
<iframe src="https://public.tableau.com/views/EstimatedIndonesianAgriculturalProductionperYear/EstimatedIndonesianAgriculturalProductionperYear?:showVizHome=no&:embed=true" width="800" height="1100"></iframe>
</center>