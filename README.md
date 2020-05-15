# BiDAF-pytorch-with-Self-Attention

Forked from [galsang/BiDAF-pytorch](https://github.com/galsang/BiDAF-pytorch) and added self-attention implementation.

Unfortunately, self-attention only make it performance better than the original version a little.

| Model(Single)                                                | EM(%)(dev) | F1(%)(dev) |
| ------------------------------------------------------------ | :--------: | :--------: |
| Baseline(original version)                                   |    64.2    |    75.4    |
| Self-Attention(with default arguments)                       |   64.882   |   75.582   |
| Self-Attention(with --hidden-size=125 --char-channel-size=150) |   65.705   |   76.442   |
| **Self-Attention(with more modeling LSTM and default arguments)** | **64.380** | **75.648** |

In my test, the baseline model did not performance as well as in  [galsang/BiDAF-pytorch](https://github.com/galsang/BiDAF-pytorch)'s test, ~~maybe I was just unlucky~~.

The model.py.bak refers to the model of row 2 and 3 in the sheet.

