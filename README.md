# TAMUDatathon2022Submission

This is my submission for the TAMU Datathon 2022 "Puzzle Solver" challenge.

# Relevant Files

There were two components to this challenge:
* Submit code to TAMU Datathon directly, for which their "autograder" would run it. In this, I included a saved reference to my best model, which would then load it and make predictions.
* The second part was actually building the best model, which is encapsulated in the `jigsaw002.ipynb` jupyter notebook.

# Approach

I thought I could get away with doing a naive heuristic where I'd, for each one of the 24 arrangements, look at the edges and calculate a distance metric, e.g., Euclidean distance. Then, I'd pick the arrangement with the lowest distance metric. This worked, but various issues crept up, e.g., the white padding surrounding would liked to be "joined" in the middle.

My naive heuristic not working, I then went down a more traditional approach, i.e., building a multinomial classifier. My classification target was one of the 24 possible arrangements.
