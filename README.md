# independentStudy

The following files are code for the Independent Study I pursued in the Spring of 2022. The goal of this project was to create a machine learning model that would read through different Reddit posts prior to an NFL game, and create a prediction as to whether a team would win or lose based on those Reddit posts.

Running the files are fairly straightforward. To acquire the data, you must run the scraping reddit file. This will get all the Reddit posts from 2021-2022 NFL season. This can be very time consuming, so the other files will reference a google drive link to the data which can be used instead.

This project is set up to have two neural nets. The first neural net is trained on individual Reddit posts, and assigns a value/weight on how likely each post is to indicate a win or loss. This model can be acquired by running the "neuralNet" file. At the bottom of the notebook, the model is then made to evaluate some new data. This is to help the next neural net. The second neural net ("weightedNet") takes the weights assigned by the first neural net, and combines them with the amount of upvotes each post has. It then sorts through all the values of all the posts leading up to a game, and makes a prediction. The file contains a function for a weighted average as well, however the neural net was found to be more accurate. 

All the files and data that were referenced in this project should be accessible using the google ID references in the code itself.
