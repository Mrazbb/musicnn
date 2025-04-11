
# musicnn

This repository is fork of the repository [jordipons/musicnn](https://github.com/jordipons/musicnn)


Pronounced as "musician", `musicnn` is a set of pre-trained musically motivated convolutional neural networks for music audio tagging. This repository also includes some pre-trained [vgg-like](https://github.com/jordipons/musicnn/blob/master/vgg_example.ipynb) baselines.

## Instaling python environment

### Installing specific python verison

```bash
brew update
brew install pyenv
pyenv install 3.8.16
```

### Creating env with specific python version
```bash
eval "$(pyenv init -)"
pyenv local 3.8.16
python -m venv musicnn_env
source musicnn_env/bin/activate
python setup.py install
pip install tensorflow-macos==2.13.0 tensorflow-metal numpy==1.24.3 librosa==0.10.2.post1 matplotlib scikit-learn pandas
```

After instalation you can choose this python env in your Jupyter python notebook as a kernel.

### Using examples
Part of this example are mainly these files:
- [tagging_example.ipynb](tagging_example.ipynb) (creates a CSV with different tags for every 3 seconds)
- [musicnn_example.ipynb](musicnn_example.ipynb) (more detailed explanation of the tagging process and how it works)


Check the [documentation](https://github.com/jordipons/musicnn/blob/master/DOCUMENTATION.md) and our [basic](https://github.com/jordipons/musicnn/blob/master/tagging_example.ipynb) / [advanced](https://github.com/jordipons/musicnn/blob/master/musicnn_example.ipynb) examples to understand how to use `musicnn`.

## Uninstaling python environment

```bash
deactivate
rm -rf musicnn_env
```


## Musicnn Example
Analysing AUDIO and outputting CSV with all features every three seconds.
[Open Musicnn Example](musicnn_example.ipynb)
![alt text](./images/Screenshot%202025-03-12%20at%2012.18.12.png "Taggram")
