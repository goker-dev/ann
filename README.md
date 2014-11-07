ann
===

###Artificial Neural Network (Backpropagation)

This is a Python Multilayer Backpropagation ANN sample. The network has __3 neurons__. The _2 inputs_ are **N1**, **N2** and _the output_ is **N3**.
It calculates neurons' weights by the signum function. It stops learning by the number of iterations or error ratio value.
It generates both text and graphical results (with decision boundaries) when the learning is finished.

####The Signum Function:

    def sigma(x):
    return 1 / (1 + math.exp(-x))

####Sample Input (XOR):

    dataset = [[0, 0, 0], [0, 1, 1], [1, 0, 1], [1, 1, 0]]

####Sample Output (XOR):

    initial weights
    ['0.30', '0.27', '0.75']
    ['0.92', '0.61', '0.54']
    ['0.98', '0.13', '0.01']
    last weights
    ['5.18', '5.13', '2.25']
    ['4.92', '4.81', '7.48']
    ['7.47', '-7.72', '3.58']
    outputs
    ['0.05', '0.96', '0.95', '0.04']
    iteration: 3420, totalError: 0.19 / 4 = 0.05
    decision boundaries (ax+by+c=0)
    5.18x + 5.13y + 2.25 = 0
    4.92x + 4.81y + 7.48 = 0
    7.47x + -7.72y + 3.58 = 0

![ANN XOR Output](https://github.com/gokercebeci/ann/blob/master/ann-output-xor.png)

####Sample Input:

    dataset = [[0.30, 3.5, 0], [0.35, 3.3, 0], [0.40, 3.6, 0], [1.20, 2.35, 0], [1.40, 2.15, 0], [1.40, 2.25, 0],
               [1.55, 2.7, 0], [2.15, 1.45, 0], [3.00, 0.65, 0], [3.40, 0.8, 0], [4.20, 1, 0], [4.25, 1.2, 0],
               [4.40, 1.45, 0], [4.60, 1.6, 0], [5.30, 1.9, 0], [5.55, 2.15, 0], [5.65, 2.2, 0], [5.85, 2.6, 0],
               [5.90, 2.75, 0], [5.95, 2.1, 0], [2.80, 1.5, 1], [2.85, 2.45, 1], [2.90, 2, 1], [3.00, 1.75, 1],
               [3.00, 2.25, 1], [3.10, 2.05, 1], [3.30, 1.55, 1], [3.35, 1.7, 1], [3.35, 1.85, 1], [3.45, 1.7, 1]]

  
####Sample Output:
  
    initial weights
    ['0.77', '0.12', '0.73']
    ['0.92', '0.25', '0.55']
    ['0.10', '0.43', '0.58']
    last weights
    ['3.53', '-5.07', '5.42']
    ['3.35', '-0.45', '7.17']
    ['-7.90', '8.03', '3.91']
    outputs
    ['0.02', '0.02', '0.02', '0.02', '0.02', '0.02', '0.03', '0.24', '0.04', '0.03', '0.02', '0.03', '0.04', '0.04', '0.03',        '0.03', '0.03', '0.06', '0.09', '0.02', '0.91', '0.91', '0.94', '0.96', '0.96', '0.97', '0.93', '0.95', '0.97', '0.95']
    iteration: 349, totalError: 1.49 / 30 = 0.05
    decision boundaries (ax+by+c=0)
    3.53x + -5.07y + 5.42 = 0
    3.35x + -0.45y + 7.17 = 0
    -7.90x + 8.03y + 3.91 = 0
    
    
![ANN Output](https://github.com/gokercebeci/ann/blob/master/ann-output.png)

License
-------
Absolutely, it is totally open source and under [MIT License](https://github.com/gokercebeci/ann/blob/master/LICENSE "MIT License") 
