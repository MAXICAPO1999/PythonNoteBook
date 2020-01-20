Análisis de Datos con python
==============
**Author:** *Jhoan Sebastian Almeida Caicedo*

***07 de enero de 2020***


```{python}

import unicodecsv

def read_csv(filename):
    with open(filename, 'rb') as f:
        reader = unicodecsv.DictReader(f)
        return list(reader)

enrollments = read_csv('enrollments.csv')
daily_engagement = read_csv('daily_engagement.csv')
project_submissions = read_csv('project_submissions.csv')
```