<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="bair_robot_pushing_small" />
  <meta itemprop="description" content="This data set contains roughly 44,000 examples of robot pushing motions, including one training set (train) and two test sets of previously seen (testseen) and unseen (testnovel) objects. This is the small 64x64 version.&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load('bair_robot_pushing_small', split='train')&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/bair_robot_pushing_small" />
  <meta itemprop="sameAs" content="https://sites.google.com/view/sna-visual-mpc/" />
  <meta itemprop="citation" content="@misc{1710.05268,&#10;  Author = {Frederik Ebert and Chelsea Finn and Alex X. Lee and Sergey Levine},&#10;  Title = {Self-Supervised Visual Planning with Temporal Skip Connections},&#10;  Year = {2017},&#10;  Eprint = {arXiv:1710.05268},&#10;}&#10;" />
</div>
# `bair_robot_pushing_small`

This data set contains roughly 44,000 examples of robot pushing motions,
including one training set (train) and two test sets of previously seen
(testseen) and unseen (testnovel) objects. This is the small 64x64 version.

*   URL:
    [https://sites.google.com/view/sna-visual-mpc/](https://sites.google.com/view/sna-visual-mpc/)
*   `DatasetBuilder`:
    [`tfds.video.bair_robot_pushing.BairRobotPushingSmall`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/video/bair_robot_pushing.py)
*   Version: `v1.0.0`
*   Versions:

    *   **`1.0.0`** (default):
    *   `2.0.0`: New split API (https://tensorflow.org/datasets/splits)

*   Size: `30.06 GiB`

## Features
```python
Sequence({
    'action': Tensor(shape=(4,), dtype=tf.float32),
    'endeffector_pos': Tensor(shape=(3,), dtype=tf.float32),
    'image_aux1': Image(shape=(64, 64, 3), dtype=tf.uint8),
    'image_main': Image(shape=(64, 64, 3), dtype=tf.uint8),
})
```

## Statistics

Split | Examples
:---- | -------:
ALL   | 43,520
TRAIN | 43,264
TEST  | 256

## Homepage

*   [https://sites.google.com/view/sna-visual-mpc/](https://sites.google.com/view/sna-visual-mpc/)

## Citation
```
@misc{1710.05268,
  Author = {Frederik Ebert and Chelsea Finn and Alex X. Lee and Sergey Levine},
  Title = {Self-Supervised Visual Planning with Temporal Skip Connections},
  Year = {2017},
  Eprint = {arXiv:1710.05268},
}
```

--------------------------------------------------------------------------------
