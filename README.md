# BIOF509-Bee-Trends

This is Kevin Oakley's final project for BIOF509 Spring 2019

My original goal was to use Machine Learning code to analyze publically available data from the USDA website (https://quickstats.nass.usda.gov) to predict trends in future Bee related census data.


After spending weeks parsing through aspects of the dataset that I acquired, I realized that it was amazingly futile for me to attempt preprocessing on such a complex dataset...at least at my present skill level.  I have included the scratch notebooks to catalog the crazy holes I dug myself looking for ways to make it work.  Disclaimer; logical order may not exist.

Ultimately, I decided that instead of forcing the collected data to fit my desires for illustrating the ML techniques introduced in this course, I had to fabricate random data with distinct features that may be relevant to Bee Hive/Colony Survival over the course of an imagined season. All of the data was generated randomly based on the values in the headers of each column.  The goal then is not to generate a model that will translate to field collected data.  I simply wasn't able to find data that I could work with for the scope of this project.   

The features are not categorical, since that is one of the major hurdles I could not overcome with the original dataset. I generated the CSV files using the Numbers spreadsheet software (Apple). I couldn't figure out how to randomize a binary list in that program, so I made a few of the columns equal to either 0 or 1, which saved me the code to encode them later.  Although this is a skill I am comfortable with, as seen in the scratch notebook.

# My project has since become to use Unsupervisd learning to train the randomized fabricated data, looking for trends that will predict survival of honey Bee colonies (hives) given the few features I generated.

I have made two randomized datasets to use for prediction.  The training data set to develop the model has 793 rows.  I will ultimately test the other Naive dataset (1050 rows) once I a model has been selected.


