---
title: "NocoDB Architecture"
description: "NocoDB Architecture Overview"
position: 4000
category: "Engineering"
menuTitle: "NocoDB Architecture"
---

By default, if `NC_DB` is not specified, then SQLite will be used to store your meta data. We suggest users to separate the meta data and user data in different databases.

<!-- TODO: update diagram -->
<img src="../architecture.png" style="background: white;border-radius:4px;padding :10px">

| Project Type | Metadata stored in | Data stored in |
|---------|-----------|--------|
| Create new project | NC_DB | NC_DB |
| Create new project with External Database | NC_DB | External Database |
| Create new project from Excel | NC_DB | NC_DB |