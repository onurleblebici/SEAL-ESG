SEAL-ESG -- An Implementation of SEAL for Event Sequence Graph Link Prediction Tasks
===============================================================================

About
-----

SEAL framework which uses sub-graphs, attributes and embedding (uses node2vec for this purpose) features of the graph. SEAL Framework extracts sub-graphs of related nodes and learns the features of these sub-graphs via DGCNN and uses the learned model for link prediction.

Original SEAL implementation is extended in some aspects as follows.
-----

Parameters of DGCNN model are hidden and couldn’t be tuned externally. The ability to tune hyperparameters of neural network is crucial. Some minor bugs are fixed which prevents the application to run on training data format except mat file format. Training, validation and test results were printed on the screen by the application. Working in this way was challenging to evaluate results between iterations. For this reason, all the results are written in a csv formatted file at the end of the each iteration.

Original SEAL implementation
-----

The original implementation of SEAL is [here](https://github.com/muhanzhang/SEAL).

The original paper of SEAL is:
> M. Zhang and Y. Chen, Link Prediction Based on Graph Neural Networks, Advances in Neural Information Processing Systems (NIPS-18). [\[PDF\]](https://arxiv.org/pdf/1802.09691.pdf)

Reference
---------

If you find the code useful, please cite our paper.

    @inproceedings{
      title={Application of Graph Neural Networks on Software Modeling},
      author={Onur Yusuf Leblebici},
      year={2020}
    }
