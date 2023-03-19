~~---
title: Cloud Software Architecture Pattern Repository
tags: [architecture,cloud]
keywords:
summary: "Repository of Cloud Software Architecture Patterns"
sidebar: mydoc_sidebar
permalink: software_design.html
folder: patterns
---
<style>
    /* body rules included when showing the example as a live example */
    body {
        background-color: #fff;
        color: #333;
        font: 1.2em / 1.5 Helvetica Neue, Helvetica, Arial, sans-serif;
        padding: 0;
        margin: 0;
    }

    img {
        max-width: 100%;
    }

    .cards {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
        grid-gap: 20px;
        max-width: 800px;
        margin: 1em auto;
    }

    .card {
        display: grid;
        grid-template-rows: max-content 200px 1fr;
        border: 1px solid #999;
        border-radius: 3px;
    }

    .card img {
        object-fit: cover;
        width: 100%;
        height: 100%;
    }

    .card h2 {
        margin: 0;
        padding: .5rem;
    }

    .card .content {
        padding: .5rem;
    }

    .card footer {
        background-color: #333;
        color: #fff;
        padding: .5rem;
    }
</style>

# Cloud Software Design Patterns

<div class="cards">
  <article class="card">
     <h2>Aggregator-style Patterns</h2>
  </article>
  <div class="content">
     <p>Ambassador, API Gateway, etc</p>
  </div>
</div>

| Pattern | Classification |
|---------|----------------|
|  <a href="api_gateway_pattern.html" class="btn btn-primary">Gateway</a>| Aggregator |
|  <a href="ambassador_pattern.html" class="btn btn-primary">Ambassador</a>| Aggregator |

