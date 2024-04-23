# Introduction

Anki users often have lots of decks for different subjects or topics. FSRS can be optimized in collection level and deck level. 

Which one is the best? How to develop a method to choose the best level relied on the data?

This repository is used to figure it out.

## Initial results

I run an experiment in two collections. The initial results show that optimization on deck level is better. 

In collection A, it reduce RMSE(bins) from 0.0219 to 0.0217 (relatively ~1%, insignificantly). In collection B, it reduce RMSE(bins) from 0.0361 to 0.0305 (relatively ~16%, significantly).

## Explanation

From the modeling perspective, it's a method like Model Ensemble, Hierarchical Modeling and Local Modeling.

From the data perspective, different materials in different topics have different memory patterns.

The initial stability can display the difference obviously. And we can also find out some other proxies, such as the button usage in the new cards.

## The next step

Are there counter-examples? How to cluster decks when local modeling results in worse metrics?
