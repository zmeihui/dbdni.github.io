---
layout: post
title:  'Cloudy with high chance of DBMS: A 10-year prediction for Enterprise-Grade ML'
date:   2020-05-06
author: Carlo Curino and Kostas Karanasos (Microsoft Jim Gray Systems Lab)
---

Machine learning (ML) has proven itself in high-value web applications such as search ranking and is emerging as a powerful tool in a much broader range of enterprise scenarios including voice recognition and conversational understanding for customer support, intelligent feedback loops in large-scale sysops, manufacturing, and autonomous vehicle management, just to name a few. Meanwhile, as the value of data is increasingly recognized and monetized, concerns about securing valuable data and risks to individual privacy have been growing. Consequently, rigorous data management has emerged as a key requirement in enterprise settings. 

In the first half of this talk, Carlo will present GSL's vision of how ML and database systems are likely to come together, and early steps we take towards making this vision a reality. In the process, he will attempt to answer the following questions: How will the trends of ML growing popularity and stricter data governance intersect? What are the unmet requirements for applying ML in enterprise settings? What are the technical challenges for the DB community to solve? 

In the second half, Konstantinos will focus on the common and consequential part of model inference. He will present Raven, a system that leverages native integration of ML runtimes (such as ONNX Runtime) deep within SQL Server, taking advantage of DBMS's mature infrastructure for fast data access and processing along with its support for enterprise features (e.g., encryption, auditing, high-availability). Raven employs a unified intermediate representation (IR) to enable advanced cross-optimizations between ML and database operators. In this optimization space, we discover the most exciting research opportunities that combine DB/compiler/ML thinking. Our initial evaluation on real data demonstrates performance gains of up to 5.5x from the native integration of ML in SQL Server, up to 24x from cross-optimizations, and orders of magnitude from conversions to tensor computations. An early preview of the ONNX Runtime integration is currently available with Azure’s SQL Database Edge.
