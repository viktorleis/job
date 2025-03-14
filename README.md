# Join Order Benchmark

This repository contains the Join Order Benchmark (JOB) queries from the [paper](https://www.vldb.org/pvldb/vol9/p204-leis.pdf):

How Good Are Query Optimizers, Really?
by Viktor Leis, Andrey Gubichev, Atans Mirchev, Peter Boncz, Alfons Kemper, Thomas Neumann
PVLDB Volume 9, No. 3, 2015

# Loading

To load the database into PostgreSQL:

1. Create the schema:

```
\i schema.sql
```

2. Download and unpack the CSV files from https://event.cwi.nl/da/job/imdb.tgz

3. Load the CSV files:

```
\copy aka_name from 'aka_name.csv' csv escape '\'
\copy aka_title from 'aka_title.csv' csv escape '\'
\copy cast_info from 'cast_info.csv' csv escape '\'
\copy char_name from 'char_name.csv' csv escape '\'
\copy comp_cast_type from 'comp_cast_type.csv' csv escape '\'
\copy company_name from 'company_name.csv' csv escape '\'
\copy company_type from 'company_type.csv' csv escape '\'
\copy complete_cast from 'complete_cast.csv' csv escape '\'
\copy info_type from 'info_type.csv' csv escape '\'
\copy keyword from 'keyword.csv' csv escape '\'
\copy kind_type from 'kind_type.csv' csv escape '\'
\copy link_type from 'link_type.csv' csv escape '\'
\copy movie_companies from 'movie_companies.csv' csv escape '\'
\copy movie_info from 'movie_info.csv' csv escape '\'
\copy movie_info_idx from 'movie_info_idx.csv' csv escape '\'
\copy movie_keyword from 'movie_keyword.csv' csv escape '\'
\copy movie_link from 'movie_link.csv' csv escape '\'
\copy name from 'name.csv' csv escape '\'
\copy person_info from 'person_info.csv' csv escape '\'
\copy role_type from 'role_type.csv' csv escape '\'
\copy title from 'title.csv' csv escape '\'
```
