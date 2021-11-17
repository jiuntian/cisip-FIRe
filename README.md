# Fast Image Retrieval
[![Documentation Status](https://readthedocs.org/projects/fast-image-retrieval/badge/?version=latest)](https://fast-image-retrieval.readthedocs.io/en/latest/?badge=latest)

Documentation: https://fast-image-retrieval.readthedocs.io/en/latest/

## Introduction
Fast Image Retrieval is an open source image retrieval framework release by Center of Image and Signal Processing Lab (CISiP Lab), Universiti Malaya. This framework implements most of the major binary hashing methods, together with different popular backbone networks and public datasets.

### Major features
- **One for All**

    Herein, we unified (i) various binary hashing methods, (ii) different backbone, and (iii) multiple datasets under a single framework to ease the research and benchmarking in this domain. It supports popular binary hashing methods, e.g. HashNet, GreedyHash, DPN, OrthoHash, etc.
- **Modularity**

    We break the framework into parts so that one can easily implement their own method by joining up the components.

## License
This project is released under [BSD 3-Clause License](https://github.com/CISiPLab/fast-image-retrieval/blob/main/LICENSE).

## Changelog
Please refer to [Changelog](https://fast-image-retrieval.readthedocs.io/en/latest/misc.html#changelog) for more detail.
## Implemented method/backbone/datasets
[//]: <> (This is copied from docs/implementation.md)
### Backbone
1. Alexnet
2. VGG{16}
3. ResNet{18,34,50,101,152}

### Loss (Method)
#### Supervised
|Method|Config Template|Loss Name|
|---|---|---|
|ADSH|adsh.yaml|adsh|
|BiHalf|bihalf-supervised.yaml|bihalf-supervised|
|Cross Entropy|ce.yaml|ce|
|CSQ|csq.yaml|csq|
|DBDH|dbdh.yaml|dbdh|
|DFH|dfh.yaml|dfh|
|DPN|dpn.yaml|dpn|
|DPSH|dpsh.yaml|dpsh|
|DTSH|dtsh.yaml|dtsh|
|GreedyHash|greedyhash.yaml|greedyhash|
|HashNet|hashnet.yaml|hashnet|
|JMLH|jmlh.yaml|jmlh|
|MIHash|mihash.yaml|mihash|
|OrthoCos(OrthoHash)|orthocos.yaml|orthocos|
|OrthoArc(OrthoHash)|orthoarc.yaml|orthoarc|
|SDH|sdh.yaml|sdh|
|SDH-C|sdhc.yaml|sdhc|
#### Unsupervised
|Method|Config Template|Loss Name|
|---|---|---|
|BiHalf|bihalf.yaml|bihalf|
|CIBHash|cibhash.yaml|cibhash|
|GreedyHash|greedyhash-unsupervised.yaml|greedyhash-unsupervised|
|SSDH|ssdh.yaml|ssdh|
|TBH|tbh.yaml|tbh|
#### Shallow (Non-Deep learning methods)
|Method|Config Template|Loss Name|
|---|---|---|
|ITQ|itq.yaml|itq|
|LsH|lsh.yaml|lsh|
|PCAHash|pca.yaml|pca|
|SH|sh.yaml|sh|



### Datasets
|Dataset|Name in framework|
|---|---|
|ImageNet100|imagenet|
|NUS-WIDE|nuswide|
|MS-COCO|coco|
|MIRFLICKR/Flickr25k|mirflickr|
|Stanford Online Product|sop|
|Cars dataset|cars|
|CIFAR10|cifar10|

## Installation
Please head up to [Get Started Docs](https://fast-image-retrieval.readthedocs.io/en/latest/get_started.html) for guides on setup conda environment and installation.

## Tutorials
Please head up to [Tutorials Docs](https://fast-image-retrieval.readthedocs.io/en/latest/tutorials.html) for guidance.

## Reference

If you find this framework useful in your research, please consider cite this project.

```
@inproceedings{dpn2020,
  title={Deep Polarized Network for Supervised Learning of Accurate Binary Hashing Codes.},
  author={Fan, Lixin and Ng, Kam Woh and Ju, Ce and Zhang, Tianyu and Chan, Chee Seng},
  booktitle={IJCAI},
  pages={825--831},
  year={2020}
}

@inproceedings{orthohash2021,
  title={One Loss for All: Deep Hashing with a Single Cosine Similarity based Learning Objective},
  author={Hoe, Jiun Tian and Ng, Kam Woh and Zhang, Tianyu and Chan, Chee Seng and Song, Yi-Zhe and Xiang, Tao},
  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
  year={2021}
}
```

## Contributing
We welcome the contributions to improve this project. Please file your suggestions/issues by creating new issues or send us a pull request for your new changes/improvement/features/fixes.
