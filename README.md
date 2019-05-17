# BIOF509-Bee-Trends

This is Kevin Oakley's final project for BIOF509 Spring 2019 FAES

My original goal was to use Machine Learning code to analyze publically available data from the USDA website (https://quickstats.nass.usda.gov) to predict trends in Honey Bee related census data.


After spending weeks parsing through aspects of the dataset that I acquired, I realized that it was amazingly futile for me to attempt preprocessing on such a complex dataset...at least at my present skill level.  I have included the scratch notebooks to catalog the crazy holes I dug myself looking for ways to make it work.  Disclaimer; logical order may not exist.

Ultimately, I decided that instead of forcing the census and survey data reported by to the USDA to fit my desires for illustrating the ML techniques introduced in this course, I would turn my attention to the smaller scale recreational beekeeping level.  My new goal was to find data that would contain observations of hives over the course of a season, including survival to the subsequent season, to determine if there are any predictors of strength/survival likelihood.

This is of particular interest because the beekeeping community has been dealing with a surplus of variables concerning hive collapse, with no strong deterministic results.  My focus is less on environmental data (pesticides, access to pollen, mosquito control, etc.) to avoid pitfalls of theoretical widescale honey bee decline.  I hoped to instead use observations that can be reported by individual beekeepers.

Unfortunately, no large datasets currently exist that hold such data.  This leads to a future project of learning how to host an online journaling site that will be able to populate the data of interest, and serve as a personal record keeping journal for the novice beekeeper. 

For this assignment however, I reluctantly chose to fabricate random data with distinct features that may be relevant to honeybee hive/colony survival over the course of an imagined season. All of the data was generated randomly based on the values in the headers of each column.  The goal then is not to generate a model that will translate to real-world field collected data since I simply wasn't able to find data that I could work with for the scope of this project.   

The features are not categorical, since that is one of the major hurdles I could not overcome with the original dataset. I generated the CSV files using the Numbers spreadsheet software (Apple). I couldn't figure out how to randomize a binary list in that program, so I made a few of the columns equal to either 0 or 1, which saved me the need to encode them later.  Although this is a skill I am comfortable with, as seen in the scratch notebook.  

After seeing that no particular feature has a predictive influence on the random data (although classifiers scored above 50%), I decided to also merge a dataset with some bias towards what I believe can influence a *stronger* hive (less pest detection, more days of sunshine, lack of swarm or generation of new queen cells, and survival) and conversely, a *weaker* hive (with values essentially inverted).  The intent is to supply more skewed data to see the effect on training models.

# My project has since become to use Unsupervised learning to train the randomized **fabricated data**, looking for trends that will predict survival of honeybee colonies (hives) given the few features I generated.

I have made two randomized datasets to use for prediction.  The training data set to develop the model has 793 rows.  I will ultimately test the other Naive dataset (1050 rows) once I a model has been selected.


