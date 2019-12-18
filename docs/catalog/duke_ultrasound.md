<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="duke_ultrasound" />
  <meta itemprop="description" content="DukeUltrasound is an ultrasound dataset collected at Duke University with a &#10;Verasonics c52v probe. It contains delay-and-sum (DAS) beamformed data &#10;as well as data post-processed with Siemens Dynamic TCE for speckle &#10;reduction, contrast enhancement and improvement in conspicuity of &#10;anatomical structures. These data were collected with support from the&#10;National Institute of Biomedical Imaging and Bioengineering under Grant &#10;R01-EB026574 and National Institutes of Health under Grant 5T32GM007171-44.&#10;A usage example is avalible &#10;[here](https://colab.research.google.com/drive/1R_ARqpWoiHcUQWg1Fxwyx-ZkLi0IZ5qs).&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('duke_ultrasound', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/duke_ultrasound" />
  <meta itemprop="sameAs" content="https://github.com/ouwen/mimicknet" />
  <meta itemprop="citation" content="@article{DBLP:journals/corr/abs-1908-05782,&#10;  author    = {Ouwen Huang and&#10;               Will Long and&#10;               Nick Bottenus and&#10;               Gregg E. Trahey and&#10;               Sina Farsiu and&#10;               Mark L. Palmeri},&#10;  title     = {MimickNet, Matching Clinical Post-Processing Under Realistic Black-Box&#10;               Constraints},&#10;  journal   = {CoRR},&#10;  volume    = {abs/1908.05782},&#10;  year      = {2019},&#10;  url       = {http://arxiv.org/abs/1908.05782},&#10;  archivePrefix = {arXiv},&#10;  eprint    = {1908.05782},&#10;  timestamp = {Mon, 19 Aug 2019 13:21:03 +0200},&#10;  biburl    = {https://dblp.org/rec/bib/journals/corr/abs-1908-05782},&#10;  bibsource = {dblp computer science bibliography, https://dblp.org}&#10;}" />
</div>
# `duke_ultrasound`

DukeUltrasound is an ultrasound dataset collected at Duke University with a
Verasonics c52v probe. It contains delay-and-sum (DAS) beamformed data as well
as data post-processed with Siemens Dynamic TCE for speckle reduction, contrast
enhancement and improvement in conspicuity of anatomical structures. These data
were collected with support from the National Institute of Biomedical Imaging
and Bioengineering under Grant R01-EB026574 and National Institutes of Health
under Grant 5T32GM007171-44. A usage example is avalible
[here](https://colab.research.google.com/drive/1R_ARqpWoiHcUQWg1Fxwyx-ZkLi0IZ5qs).

*   URL:
    [https://github.com/ouwen/mimicknet](https://github.com/ouwen/mimicknet)
*   `DatasetBuilder`:
    [`tfds.image.duke_ultrasound.DukeUltrasound`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/image/duke_ultrasound.py)
*   Version: `v1.0.0`
*   Versions:

    *   **`1.0.0`** (default):

*   Size: `12.78 GiB`

## Features
```python
FeaturesDict({
    'das': FeaturesDict({
        'dB': Tensor(shape=(None,), dtype=tf.float32),
        'imag': Tensor(shape=(None,), dtype=tf.float32),
        'real': Tensor(shape=(None,), dtype=tf.float32),
    }),
    'dtce': Tensor(shape=(None,), dtype=tf.float32),
    'f0_hz': Tensor(shape=(), dtype=tf.float32),
    'final_angle': Tensor(shape=(), dtype=tf.float32),
    'final_radius': Tensor(shape=(), dtype=tf.float32),
    'focus_cm': Tensor(shape=(), dtype=tf.float32),
    'harmonic': Tensor(shape=(), dtype=tf.bool),
    'height': Tensor(shape=(), dtype=tf.uint32),
    'initial_angle': Tensor(shape=(), dtype=tf.float32),
    'initial_radius': Tensor(shape=(), dtype=tf.float32),
    'probe': Tensor(shape=(), dtype=tf.string),
    'scanner': Tensor(shape=(), dtype=tf.string),
    'target': Tensor(shape=(), dtype=tf.string),
    'timestamp_id': Tensor(shape=(), dtype=tf.uint32),
    'voltage': Tensor(shape=(), dtype=tf.float32),
    'width': Tensor(shape=(), dtype=tf.uint32),
})
```

## Statistics

Split      | Examples
:--------- | -------:
ALL        | 6,248
TRAIN      | 2,556
A          | 1,362
B          | 1,194
TEST       | 438
MARK       | 420
VALIDATION | 278

## Homepage

*   [https://github.com/ouwen/mimicknet](https://github.com/ouwen/mimicknet)

## Supervised keys (for `as_supervised=True`)
`(u'das/dB', u'dtce')`

## Citation
```
@article{DBLP:journals/corr/abs-1908-05782,
  author    = {Ouwen Huang and
               Will Long and
               Nick Bottenus and
               Gregg E. Trahey and
               Sina Farsiu and
               Mark L. Palmeri},
  title     = {MimickNet, Matching Clinical Post-Processing Under Realistic Black-Box
               Constraints},
  journal   = {CoRR},
  volume    = {abs/1908.05782},
  year      = {2019},
  url       = {http://arxiv.org/abs/1908.05782},
  archivePrefix = {arXiv},
  eprint    = {1908.05782},
  timestamp = {Mon, 19 Aug 2019 13:21:03 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/corr/abs-1908-05782},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

--------------------------------------------------------------------------------
