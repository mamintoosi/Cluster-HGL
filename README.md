Cluster-HGL
==========
 [![repo size](https://img.shields.io/github/repo-size/mamintoosi/Cluster-HGL.svg)](https://github.com/mamintoosi/Cluster-HGL/archive/master.zip)
 [![GitHub forks](https://img.shields.io/github/forks/mamintoosi/Cluster-HGL)](https://github.com/mamintoosi/Cluster-HGL/network)
[![GitHub issues](https://img.shields.io/github/issues/mamintoosi/Cluster-HGL)](https://github.com/mamintoosi/Cluster-HGL/issues)
[![GitHub license](https://img.shields.io/github/license/mamintoosi/Cluster-HGL)](https://github.com/mamintoosi/Cluster-HGL/blob/main/LICENSE)
 
 
A PyTorch implementation of "" (Submitted)
<p align="center">
  <img width="600" src="images/">
</p>

### Abstract

<p align="justify">
AbstractCluster-GCN, in average.
</p>

This repository provides a PyTorch implementation of Cluster-HGL as described in the submitted paper:

> TO DO
> Mahmood Amintoosi,
> JAC, 2021

### Requirements
The codebase is implemented in Python 3.7.11 on Google colab. package versions used for development are just below.
```
torch-scatter 		2.0.8
torch-sparse		0.6.11
torch-geometric		2.0.1
texttable		1.6.4
karateclub		1.2.1
```

### Run on Google Colab
https://colab.research.google.com/github/mamintoosi/Cluster-HGL/blob/master/OverlappingClusterGCN.ipynb

### Datasets
<p align="justify">
We used some of the citation network datasets, which are accessible from <a href=https://pytorch-geometric.readthedocs.io/en/latest/modules/datasets.html>
PyTorch-geometric </a>
</p>

#### Model options
```
  --clustering-method   STR     Clustering method.             Default is `DANMF`.
  --cluster-number      INT     Number of clusters.            Default is 2x Number of dataset labels. 
  --seed                INT     Random seed.                   Default is 42.
  --epochs              INT     Number of training epochs.     Default is 10.
  --test-ratio          FLOAT   Training set ratio.            Default is 0.3.
  --learning-rate       FLOAT   Adam learning rate.            Default is 0.01.
  --dropout             FLOAT   Dropout rate value.            Default is 0.5.
  --layers              LST     Layer sizes.                   Default is [16, 16, 16]. 
  --membership-closeness FLOAT  WMC parameter					Default is 0.1
  --dataset-name		STR		Dataset Name					Default is Cora
```
-------------------------------------------------------

This code is heavily borrowed from <a href="https://github.com/benedekrozemberczki/ClusterGCN">ClusterGCN</a>