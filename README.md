# puzzle-piece-classification
Originally to answer https://stackoverflow.com/questions/36703964/want-to-detect-edge-and-corner-parts-in-a-jigsaw-puzzle-but-cant-find-the-4-co.
The goal is to classify puzzle pieces in border/corner/center, basing on an image.
No machine learning is used: just peak/valleys analysis on the function that describes the distance of the piece's contour from the center of the enclosing circumnference.
The number of "knobs" is the number of maxima - 4 (provided adequate function regularity given by smoothing), and the number of "holes" is the number of minima under a cretain threhsold. From there, it's easy to classify the type of piece.
