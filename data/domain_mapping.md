This file describes the fields in the `topics.csv` file, a tidy CSV 
table that maps regular expressions, that when matched against a domain name,
returns a country code and sector code for that domain (or "" if undetermined).

### Field description {-}

  * `tag` (string): A single-word name for the topic (key field).
  * `areas` (string): A descriptive list of the areas covered by this topic.
  * `color` (string): An RGB color value to show this topic graphically
  * `contrast` (string): A named background color to provide contrast against color.
