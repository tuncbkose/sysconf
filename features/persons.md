The file `persons.csv` contains aggregated information about all authors, TPC chairs, and other roles in the selected conference subset.
The data was generated by `/home/eitan/Dropbox/code/sysconf/src/gather_persons.py` from git hash 63978c7


### Field description {-}

  * `name` (string): Full person name, normalized and quoted.
  * `gs_email` (string): The email affiliation of the author as reported by GS (latest).
  * `gender` (categorical string): Verified or inferred gender.
  * `country` (categorical string): Two-letter country code from email affiliation (either paper or GS).
  * `sector` (categorical string): Employer sector from email affiliation (either paper or GS).
  * `npubs` (int): Author's total publications (minimum across all conferences).
  * `hindex` (int): Author's H-index (minimum).
  * `hindex5y` (int): Author's H-index for past 5 years (minimum).
  * `i10index` (int): Author's i10 index (minimum).
  * `i10index5y` (int): Author's i10 index for past 5 years (minimum).
  * `citedby` (int): Author's total citations (minimum).