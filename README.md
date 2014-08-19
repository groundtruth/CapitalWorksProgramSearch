LoddonCapitalWorksProgramSearch
===============================

Search widget for the Loddon capital works program spreadsheet

# Backend: CSV preparation

The CSV file is prepared by:
1) exporting the tab 'Works Program' from the overall spreasheet,
2) removing the header lines,
3) renaming it to "WorksProgram.csv",
4) committing it at "data/" in this repository.

# Front-end: widget integration

* A useful setting is to add compression of 'text/csv' on the web server.
In Apache2, it can be done in `/etc/apache2/mods-enabled/deflate.conf`:
    `AddOutputFilterByType DEFLATE text/csv`
* Recommended minimum size for embedding (e.g. in an iframe) is:
  * width:  650px
  * height: 300px
