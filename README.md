char-rnn-deeplearnjs
===


Multi-layer Recurrent Neural Networks (LSTM, RNN) for character-level language models in Javascript using deeplearnjs

Inspired from  [Karpathy's char-rnn](https://github.com/karpathy/char-rnn).

and by   [sherjilozair char-rnn](https://github.com/sherjilozair/char-rnn-tensorflow)


Deeplearnjs github at [https://github.com/PAIR-code/deeplearnjs](https://github.com/PAIR-code/deeplearnjs)


The char-rnn was brought up as an issue at [https://github.com/PAIR-code/deeplearnjs/issues/237](https://github.com/PAIR-code/deeplearnjs/issues/237)


Oct 29, 2017

Just getting started on converting this to deeplearnjs

any help would be appreciated


A good starting point is to probably port the tensorflow model into your web page

Here is how to do it with Typescript

https://deeplearnjs.org/demos/mnist/mnist.html




.




.




.





.





.








The old readme file 

## Requirements
- [Tensorflow 1.0](http://www.tensorflow.org)

## Basic Usage
To train with default parameters on the tinyshakespeare corpus, run `python train.py`. To access all the parameters use `python train.py --help`.

To sample from a checkpointed model, `python sample.py`.

## Datasets
You can use any plain text file as input. For example you could download [The complete Sherlock Holmes](https://sherlock-holm.es/ascii/) as such:

```bash
cd data
mkdir sherlock
cd sherlock
wget https://sherlock-holm.es/stories/plain-text/cnus.txt
mv cnus.txt input.txt
```

Then start train from the top level directory using `python train.py --data_dir=./data/sherlock/`

A quick tip to concatenate many small disparate `.txt` files into one large training file: `ls *.txt | xargs -L 1 cat >> input.txt`

## Tensorboard
To visualize training progress, model graphs, and internal state histograms:  fire up Tensorboard and point it at your `log_dir`.  E.g.:
```bash
$ tensorboard --logdir=./logs/
```

Then open a browser to [http://localhost:6006](http://localhost:6006) or the correct IP/Port specified.


## Roadmap
- [ ] Add explanatory comments
- [ ] Expose more command-line arguments
- [ ] Compare accuracy and performance with char-rnn
- [ ] More Tensorboard instrumentation

## Contributing
Please feel free to:
* Leave feedback in the issues
* Open a Pull Request
* Join the [gittr chat](https://gitter.im/char-rnn-tensorflow/Lobby)
* Share your success stories and data sets!
