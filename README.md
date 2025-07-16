# UniKey - Enabling Surface-Based Typing with Commodity Smartwatches via Cross-Modal Learning

This repository holds a reference proof-of-concept implementation for UniKey, which enables surface-based typing via analysis of coarse grained temporal and spatial features. 

Link to paper: [ACM OPEN ACCESS](TBC)

## Note - This repository is under construction
We are currently still in the process of open sourcing UniKey, which will take some time. Please check back later for updates. We thank you for your patience.


## Overview
UniKey uses coarse grained temporal features (i.e., inter-keystroke-timings) and coarse grained spatial features (i.e., which hand was responsible for the keystroke) to infer the word being typed on a surface using a commodity smartwatch.

Briefly, UniKey works by learning a user's typing patterns through a classifier that is trained on the inter-keystroke timings (IKT) and approximate location of the keystroke (left or right hand) from a regular keyboard. This classifier is then applied to actual IKTs and L-R data collected from a smartwatch worn on the user's wrist while they type on a surface, where it leverages the learned patterns to predict the word being typed. The classifier's results are then refined using a language model (LLM) to improve accuracy and handle ambiguities in the predictions, before being presented to the user.

## Citation

If you find this work useful, please cite the following:
```
TBC
```

## License

TBC


## Contact

For any questions, or if you have any comments or feedback, there are two ways to reach out.

- File a GitHub issue under this repo.
- Drop an email to `strx [at] nus [dot] edu [dot] sg`.
