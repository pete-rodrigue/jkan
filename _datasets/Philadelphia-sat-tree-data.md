---
schema: default
title: Philadelphia Street Trees, satellite derived
organization: City of Philadelphia
notes: >-
  This data set contains information on Philadelphia's street trees, derived from satellite imagery.
resources:
  - name: Shapefile
    url: >-
      https://phl.carto.com/api/v2/sql?q=SELECT+*+FROM+ppr_tree_canopy_outlines_2015&filename=ppr_tree_canopy_outlines_2015&format=shp&skipfields=cartodb_id
    format: shp
  - name: CSV data
    url: >-
      https://phl.carto.com/api/v2/sql?q=SELECT+*,+ST_Y(the_geom)+AS+lat,+ST_X(the_geom)+AS+lng+FROM+ppr_tree_canopy_outlines_2015&filename=ppr_tree_canopy_outlines_2015&format=csv&skipfields=cartodb_id,the_geom,the_geom_webmercator
    format: csv
  - name: Metadata
    url: >-
      https://www.opendataphilly.org/dataset/ppr-tree-canopy
    format: html
license: ''
category:
  - Environment
maintainer: Chris Park
maintainer_email: chris.park@phila.gov
---
