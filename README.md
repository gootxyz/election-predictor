# Predicting the 2024 Mexican Presidential Elections

Polling has increasingly transformed into a political weapon in Mexico throughout the recent years. It has given both political parties and politicians a reason to either encourage people to vote or convince them there is no reason to do so. As any level of elections approaches, different pollsters with different methodologies claim to have the most accurate prediction of what the general public will act like in the ballots. However, inconsistent results have been a norm among the variety of organizations conducting polls in Mexico.

More recently, polls in Estado de Mexico, one of the states that concentrates the most amount of people in the country and which remains a “key” to the federal election of next year, continually announced a 25-point margin between the two candidates involved in the process days before the voting was conducted. These results were used by the candidate “leading” the race to tell those who remained undecided there was no real change to be made with their vote. The result? An eight-point final count which resulted in a victory by the candidate that was announced to have an enormous 25-point difference once. Would that result have changed if more accurate predictions were made public? This still remains one of the keys to that election.

This is the idea behind the project we are trying to implement. Based on Kellyton Brito and  Paulo Leitao’s work, which implemented a new approach to predict an election vote share based on the amount of interaction the different candidates receive on social media, and not in regards to the number of comments talking about them. The method is simple yet different from most of the literature: associating the number of likes, comments, and shares that candidates receive in their social media posts as a direct representation of the number of people who notice their online presence. This data is associated with the results of published polls to assign a vote share percentage to the number of interactions each candidate receives, and therefore, predict this vote share for any given day considering the new incoming social media data.

This data is fed to different regression models to predict the results based of new election dates, not implemented yet in unknown results. This is the ultimate goal of the project: to provide a new alternative to pollsters in Mexico which consistently show significant errors just weeks apart from each other. In this way, we aim to make inconsistent gaps of percentage difference among candidates more evident while comparing those results with our own predictions.

If proven effective, this method may be implemented to conduct consistent predictions and would welcome many more indicators, outside social media interactions, which are backed by solid theoretical research on their impact on an election´s vote share.

## Repository Description
1. [Claudia](./claudia/): Sheinbaum´s datasets
2. [Gálvez](./galvez/): Gálvez´s datasets
3. [Database Notebook](./dbCreation.ipynb): This notebook performs the extraction of the different datasets that will feed the regression models based of the [main database](./New_DB.xlsx)
4. [Prediction Notebook](./predicting.ipynb): The notebook containing all the different tests, and predictions based of the processed datasets described above.
5. [Sample Dataset](./sample.png): The overall structure of the desired datasets to feed the models
