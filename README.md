# jsmf-raw

Joint Stochastic Matrix Factorization (JSMF) for the Rectified Anchor Word (RAW) algorithm.

Co-occurrence information is powerful statistics that can model various discrete objects by their joint instances with other objects. Transforming unsupervised problems of learning low-dimensional geometry into provable decompositions of co-occurrence information, spectral inference provides fast algorithms and optimality guarantees for non-linear dimensionality reduction and latent topic analysis. Spectral approaches reduce the dependence on the original training examples, thereby producing substantial gain in efficiency, but at costs:

- The algorithms perform poorly on real data that does not necessarily follow underlying models.
- Users can no longer infer information about individual examples, which is often important for real-world applications.
- Model complexity rapidly grows as the number of objects increases, requiring a careful curation of the vocabulary.

The first issue is called model-data mismatch, which is a fundamental problem common in every spectral inference method for latent variable models. As real data never follows any particular computational model, this issue must be addressed for practicality of the spectral inference beyond synthetic settings.

The rectification paradigm in this code provides a neat solution to handle model-data mismatch not making more complex models but transforming data to a point in the space of ideal posterior. 


# Reference
[Main paper]
- https://papers.nips.cc/paper/5970-robust-spectral-inference-for-joint-stochastic-matrix-factorization.pdf

[Background paper]
- https://www.aclweb.org/anthology/D14-1138

[Related work]
- https://arxiv.org/abs/1212.4777
- https://arxiv.org/abs/1204.1956
