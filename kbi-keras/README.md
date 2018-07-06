# Joint Matrix-Tensor Factorization for Knowledge Base Inference
Code for our IJCAI 2018 Submission titled "Mitigating the Effect of Out-of-Vocabulary Entity Pairs in Matrix Factorization for KB Inference" ([arXiv2017](https://arxiv.org/pdf/1706.00637.pdf))

Joint Matrix-Tensor Factorization for Knowledge Base Inference, Prachi Jain*, Shikhar Murty*, Mausam, Soumen Chakrabarti  (*Equal Contribution)

# Running instructions
First clone the repository:
```
https://github.com/dair-iitd/KBI.git
```

Make sure you have Keras by running:
```
sudo pip install keras
```
Also, ensure you have the latest versions of both **Theano** and **numpy**.


To run the atomic models(where every relation is considered as an atom), for example DistMult, E or TransE, run the following:

```
./run.sh <dataset> <model> atomic
```
where MODEL can be **distMult**, **E** , **complex** , **TransE**, DATASET is **wn18**, **fb15k**, **fb15k-237**, **nyt-fb** and OPTIMIZER is
either **Adagrad** or **RMSprop**


To create training data, run
```
dump_data.py 
```

and  for creating data for MF, run 
```
dump_data_pairwise.py 
```

with the right set of parameters. (For info on parameters, run dump_data.py -h)

For the datasets, please contact the authors. 

