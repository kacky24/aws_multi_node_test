# AWS multi node test
- Pytorch example to train on MNIST with multiple nodes in AWS.

## Environment
- python 3.7.4

## How to run
1. Build more than two instances in AWS EC2
2. Configure security group(https://pytorch.org/tutorials/beginner/aws_distributed_training_tutorial.html)
3. Edit master address and master port in main functions of both node0.py and node1.py
4. Run node0.py in node0 and node1.py in node1
  - example
    - node0: python node0.py -n 2 -g 2 -nr 0
    - node1: python node1.py -n 2 -g 2 -nr 1

## Environment
- python 3.7.4

### Reference
- https://yangkky.github.io/2019/07/08/distributed-pytorch-tutorial.html
- https://pytorch.org/tutorials/beginner/aws_distributed_training_tutorial.html
