# Towards identifying drug side effects from social media using active learning and crowd sourcing

Implementation of an active semi-supervised VAE under representativeness constraints. Accepted in Pacific Symposium for Biocomputing (PSB) 2020.

This project applies a semi-supervised VAEs on pool-based uncertainty active learning. 
To respect the underlying class distribution different representativeness strategies can be added.

We use this architecture to find self-experiential side-effects in tweets with Amazon Mechanical Turk.

# Requirements
Requieres python 3.6+ and tensorflow-1.12+
# Project Structure
    |
    |--data:  db.zip
    |         drug_searchterm_map.csv: Contains drugnames and their coresponding searchterms.
    |         word_vec_side_effects.txt: Contains side effect synonyms.
    |--src
        |--bag_of_words: Contains tweet preprocessing (tweet tagger http://www.cs.cmu.edu/~ark/TweetNLP/#%23parser_down and 
        |        Lucene are requiered) for bag of word representation.
        |
        |--experiments: Contains code to compare VAE with other methods.
		|
		|-active_learning.py: Executes active VAE under representativeness constraints.

           
