# NBA Player Statistics ETL

## PROJECT SUMMARY

To combine all accessible many datasets on Kaggle to create a comprehensive database of information about every NBA player that was active during the 2018-2019 season.

## POST-MORTEM

### Final record count: 643

With working with large datasets from multiple sources, one of the biggest challenges faced is confirming the integrity and compatibility of each set. Our final database includes many NaN values, as the hobbyist data from data.world were found to be incomplete and/or outdated.

During transformation, mid-season trades proved to bloat the data beyond the 550 active players in the 2018-19 season. Some players appear in our dataset with one or more records and differing statistics but duplicate biographical data. For the next iteration of this project, we would separate the single master dataset in SQL as the following tables:

1) PLAYER STATISTICS + UNIFORM NUMBER
1) BIO + TATTOO
1) SALARIES
