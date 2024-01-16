# Introduction

Anki users often have lots of decks for different subjects or topics. FSRS can be optimized in collection level and deck level. 

Which one is the best? How to develop a method to choose the best level relied on the data?

This repository is used to figure it out.

## Initial results

I run an experiment in two collections. The initial results show that optimization on deck level is better. 

In collection A, it reduce RMSE(bins) from 0.0124 to 0.0111 (relatively ~10%). In collection B, it reduce RMSE(bins) from 0.0384 to 0.0323 (relatively ~16%).

## Explanation

From the modeling perspective, it's a method like Model Ensemble, Hierarchical Modeling and Local Modeling.

From the data perspective, different materials in different topics have different memory patterns.

The initial stability can display the difference obviously. And we can also find out some other proxies, such as the button usage in the new cards.

## The next step

Are there counter-examples? How to cluster decks when local modeling results in worse metrics?
