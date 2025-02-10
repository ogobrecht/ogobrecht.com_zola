+++
title = "Data Model Explorer"
description = "New in an Oracle project? Visually explore unknown data models with an APEX app!"
weight = 1
template = "page.html"

[taxonomies]
tags = ["Oracle", "APEX", "App", "Data model", "PL/SQL"]

[extra]
local_image = "/img/data-model-explorer-square.png"
+++

New in an Oracle project? Visually explore unknown data models with an APEX app!

![Scrrenshot of the running app](/img/data-model-explorer.png)

#### [View Source](https://github.com/ogobrecht/data-model-explorer){.centered-text}

## Features

- A network visualization of your own or other data models (schema tables),
  which were granted to you
- A split view screen with an overview pane on the left and an details pane
  on the right
- You can click tables in the data model visualization in the overview pane
  to directly show the details of it in the details pane
  - This works also for all other objects in the reports of the overview pane
- You can filter for multiple objects or columns (separated by spaces, works
  like a contains filter)
- You can also exclude multiple objects in the same way (think about heavily
  referenced lookup tables) to make your data model easier to read
- The tabs and select lists in the overview and details pane are showing
  numbers to help you to get as much information as possible without
  additional clicks
- The generic interactive data report in the details pane respects the data
  type of the table/view columns
  - You are able to use filters for numbers or dates, its not an simple "all
    strings" report
  - The downside of this generic approach is, that it makes more or less no
    sense to save reports or charts (they would only work for a specific
    table/view)
  - The focus is clearly on exploring your data model, see some data and have
    the possibility to filter/sort in a data type specific way
- Data Model Explorer uses two other projects in the background
  - For the visualization: [APEX plug-in "D3 Force Network
    Chart"](/projects/d3-force-apex-plugin)
  - For materialize view generation and the generic interactive report:
    [Helper packages "Data Model
    Utilities"](/projects/model)
