# PyTorch VAE Porting Challenge

Welcome to Determined AI!

Today we have a fun exercise for you. You will training a VAE model on MNIST
using Determined's training platform. For this challenge, review PyTorch's
existing VAE example. Then, port it to Determined's PyTorchTrial API and submit
the experiment to a Determined cluster.

## To Get Started

Set up the virtual environment.
```
python3.7 -m venv ~/.virtualenvs/interview
. ~/.virtualenvs/interview/bin/activate
pip install torch torchvision six
```

Add the following to model_def.py to download MNIST.
```
from six.moves import urllib
opener = urllib.request.build_opener()
opener.addheaders = [('User-agent', 'Mozilla/5.0')]
urllib.request.install_opener(opener)
```


