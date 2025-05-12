---
layout: post
title: "Using LLMs to improve search results"
date: 2024-12-1
categories: [blog]
tags: [RAG, LLM, Clustering, Search]
---

### Case study on Jahez food items search 

Jahez’s current item search system focuses on delivering exact matches for user queries, which works well for specific requests but falls short in supporting broader exploration or discovery. For instance, a search for “pepperoni pizza” might miss out on showcasing related options like other pizza varieties or complementary items that align with the user’s preferences.

To solve this, I have built a dynamic, category-based item search system built from the ground up. Products are first **grouped into smaller, meaningful clusters** based on shared characteristics like names and descriptions using **semantic embeddings**. These clusters are then merged into broader categories by applying **hierarchical clustering**, capturing diverse themes like “Classic Pizzas” or “Cheesy Favorites.” At the final stage, **Retrieval-Augmented Generation (RAG)** is used to create intuitive and user-friendly names for these categories, ensuring clarity and alignment with user expectations.

**....You can read more here, [Full Article](https://yasirmalmutauri.substack.com/p/expanding-search-moving-beyond-narrow "Substack")**