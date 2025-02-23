+++
title = "Table API Generator v0.5.0 Available"
date = "2018-12-26"
description = "Long changelog and took a long time "
slug = "table-api-generator-v0.5.0-available"
aliases = ["/posts/2018-12-26-table-api-generator-v0.5.0-available/"]

[taxonomies]
tags = ["Oracle", "PL/SQL", "Generator", "oddgen"]
+++

Short before Christmas André and I released version 0.5.0 of our [PL/SQL table API generator](https://github.com/OraMUC/table-api-generator). It took a long time to come to this point. One of the reasons behind was the fact that we had to rework some internals to support feature wishes from the community. Here the most important features of the new version:

- Support for multicolumn primary keys
- Support for 12c long identifier names
- More control over the API features and name (10 new parameters)
- Insert methods:
  - Can have the dictionary column defaults
  - Can return the whole row instead of the primary key
- You can exclude columns (e.g. audit columns) for inserts and updates
- Improved template engine:
  - Generated code better readable because of formatted parameter lists
  - Tables with many columns no longer breaking character limits
- Special methods for testing and dummy data generation
- Also see the [full changelog on the project site](https://github.com/OraMUC/table-api-generator/blob/master/docs/changelog.md#050-2018-12-23)

Happy new year and happy coding :-)

Ottmar
