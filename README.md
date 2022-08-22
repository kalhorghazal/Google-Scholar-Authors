# Google-Scholar-Authors

This <a href="https://drive.google.com/drive/folders/1v9nkcG2QasMX54Ejv2jVEpX_5DzB8xt2?usp=sharing">link</a> contains the datasets of 850,827 authors of Google Scholar we collected in 2021 and analyzed in this paper:

Title: "A new insight to the analysis of co-authorship in Google Scholar"

Authors: Ghazal Kalhor, Amin Asadi Sarijalou, Niloofar Sharifi Sadr, Behnam Bahrak

DOI: https://doi.org/10.1007/s41109-022-00460-4

If you use this dataset in your work, please cite our paper:

Kalhor, G., Asadi Sarijalou, A., Sharifi Sadr, N. et al. A new insight to the analysis of co-authorship in Google Scholar. Appl Netw Sci 7, 21 (2022). https://doi.org/10.1007/s13278-020-00695-y

# Dataset

We collected the following information for each author from Google Scholar:

* Author ID
* Institute ID
* Citation Count
* h-index
* Gender
* Country
* Fields of Interest
* Co-authors IDs


```python
import pandas as pd

authorsFeatures = pd.read_csv('authorsFeatures.csv')
authorsFeatures.head(3)
```

|Author ID|Institute ID|Citation Count|h-index|Gender|Country|
|----|----|----|----|----|----|
|QcRldecAAAAJ| 17508113656414128510|	1280|	    16|	  male|	ID|
|rkKMIwMAAAAJ|	4065822778065209794|	1280|    	16|	  male|	US|
|AUb2dK4AAAAJ|	4396926741242628134|	1280|	    16|	female|	US|

```
authorsFields = pd.read_csv('authorsFields.csv')
authorsFields.head(3)
```

|Author ID|Field of Interest|
|----|----|
|QcRldecAAAAJ|               Physics and Astronomy|
|rkKMIwMAAAAJ|	                  Computer Science|
|AUb2dK4AAAAJ|Agricultural and Biological Sciences|

```
coauthorship = pd.read_csv('coauthorship.csv')
coauthorship.head(3)
```

|Author ID|Co-author ID|
|----|----|
|rkKMIwMAAAAJ| ZjDFiYsAAAAJ|
|rkKMIwMAAAAJ| rcW8mi0AAAAJ|
|rkKMIwMAAAAJ| n07X8FoAAAAJ|
