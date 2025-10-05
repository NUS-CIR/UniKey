# UniKey - Enabling Surface-Based Typing with Commodity Smartwatches via Cross-Modal Learning

This repository holds a reference proof-of-concept implementation for UniKey, which enables surface-based typing via analysis of coarse grained temporal and spatial features. 

Link to paper: [ACM OPEN ACCESS](https://doi.org/10.1145/3746059.3747611)

## Note - This repository is under construction
We are currently still in the process of open sourcing UniKey, which will take some time. Please check back later for updates. We thank you for your patience.


## Overview
UniKey uses coarse grained temporal features (i.e., inter-keystroke-timings) and coarse grained spatial features (i.e., which hand was responsible for the keystroke) to infer the word being typed on a surface using a commodity smartwatch.

Briefly, UniKey works by learning a user's typing patterns through a classifier that is trained on the inter-keystroke timings (IKT) and approximate location of the keystroke (left or right hand) from a regular keyboard. This classifier is then applied to actual IKTs and L-R data collected from a smartwatch worn on the user's wrist while they type on a surface, where it leverages the learned patterns to predict the word being typed. The classifier's results are then refined using a language model (LLM) to improve accuracy and handle ambiguities in the predictions, before being presented to the user.

## Citation

If you find this work useful, please cite the following:
```
@inproceedings{10.1145/3746059.3747611,
author = {Tan, Sean Rui Xiang and Chan, Mun Choon and Han, Jun},
title = {UniKey: Enabling Surface-Based Typing with Commodity Smartwatches via Cross-Modal Learning},
year = {2025},
isbn = {9798400720376},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi-org.libproxy1.nus.edu.sg/10.1145/3746059.3747611},
doi = {10.1145/3746059.3747611},
abstract = {With the rise of mobile technologies such as augmented and virtual reality (AR/VR) and wearables, as well as smart TVs, the large form factor of traditional keyboards is becoming increasingly impractical. Sensing typing on surfaces offers a potential alternative, but most current solutions rely on either expensive, custom hardware or extensive user bootstrapping and calibration. In this paper, we envision Unikey, an approach to surface-based typing that uses only a commodity smartwatch to detect finger taps on a flat surface. By seamlessly adapting to the user’s existing typing habits on conventional keyboards, Unikey eliminates the need for both specialized equipment and burdensome sensor data collection, reducing overhead for users. To demonstrate the feasibility of our approach, we implement a proof-of-concept and evaluate our technique with comprehensive real-world experiments under varying conditions. Participants were invited to type while wearing smartwatches, resulting in over 2,700 minutes of recorded typing. Our experiments show that Unikey can achieve an equivalent average top-5 word error rate of 6.45\%, indicating a potential solution simple, everyday text-entry tasks.},
booktitle = {Proceedings of the 38th Annual ACM Symposium on User Interface Software and Technology},
articleno = {64},
numpages = {16},
keywords = {Text entry, ubiquitous computing, virtual reality, smartwatch, keystroke dynamics},
location = {
},
series = {UIST '25}
}
```

## Contact

For any questions, or if you have any comments or feedback, there are two ways to reach out.

- File a GitHub issue under this repo.
- Drop an email to `strx [at] nus [dot] edu [dot] sg`.
