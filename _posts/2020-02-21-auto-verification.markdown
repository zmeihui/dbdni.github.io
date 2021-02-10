---
layout: post
title:  Automatic Verification of Database-powered Workflows
date:   2020-02-21
author: Allessandro Gianola (Visitng PhD student from Free University of Bolzano)
---

During the last two decades, a huge body of research has been dedicated to the challenging problem of reconciling data and process management within contemporary organizations.  This requires to move from a purely control-flow understanding of business processes to a more holistic approach that also considers how data are manipulated and evolved by the process.
In parallel, a flourishing series of results has been dedicated to the formalization of such integrated models (e.g., the well-known artifact-centric systems), and on the boundaries of decidability and complexity for their static analysis and verification.

In this talk, I will present the verification problem of RASs (Relational Artifact Systems) - a general integrated model for artifact systems that contains the typical ingredients found in the literature - to assess (parameterized) safety properties irrespectively of the initial database instance. Such artifact systems are seen as array-based systems: the last is a model-theoretic framework that allows to employ model checking techniques based on Satisfiability Modulo Theories (SMT) by adapting the backward reachability procedure in a full-fledged declarative setting. By using suitable forms of quantifier elimination, backward reachability can be proved to be sound and complete for checking safety, and interesting fragments where backward reachability is a full decision procedure can be isolated. Moreover, the SMT technology can be exploited in implementations, building on the well-known MCMT model checker for array-based systems, and extending it to make all the foundational results fully operational.

Finally, I will present the model of DABs – a data-aware extension of BPMN where the process operates over case and persistent data. The model trades off between expressiveness and the possibility of supporting parameterized verification of safety properties on top of it. By reducing the verification problem of DABs to the one over RASs, I will discuss how the backward reachability procedure is sound and complete also for checking safety of DABs, and single out additional conditions in order to guarantee that it becomes a full decision procedure.
