# Introduction

Anki users often have lots of decks for different subjects or topics. FSRS can be optimized in collection level and deck level. 

Which one is the best? How to develop a method to choose the best level relied on the data?

This repository is used to figure it out.

## Initial results

I run an experiment in two collections. The initial results show that optimization on deck level is better sometimes.

In collection A, it increases RMSE(bins) from 0.0216 to 0.0220 (relatively ~1.85%, insignificantly). In collection B, it reduces RMSE(bins) from 0.0349 to 0.0290 (relatively ~16.9%, significantly).

## Explanation

From the modeling perspective, it's a method like Model Ensemble, Hierarchical Modeling or Local Modeling.

From the data perspective, different materials in different topics have different memory patterns.

The initial stability can display the difference obviously. And we can also find out some other proxies, such as the button usage in the new cards.

## The next step

Are there counter-examples? How to cluster decks when local modeling results in worse metrics?
