

# Synthetic Datasets

## Installation

```
pip install synthetic-datasets
```

## Datasets

* NoiseCircle


### NoiseCircle

A generator of square images, by default 64x64, with static noise and a circle
with noisy pixels in the image at a random location and with a random size.

Each result from the generator is a square numpy matrix of type float32

Example use::

```python
    from synthetic_datasets import NoiseCircle

    nc = NoiseCircle(batch_size=32, dim=64)
    for samples, labels in nc:

        // samples  is a (32, 64, 64) numpy array of noise circle images
        // labels   is a dict with three keys, "X", "Y", and "R".
        //          These represent the X, Y, and RADIUS (in pixels) of the circle in the image.
        //          Each key holds a numpy array of shape (32,)
```



## Licence
MIT


## More info
- https://github.com/synthetic-datasets/synthetic-datasets
- https://www.meetup.com/Toronto-AI/
- http://torontoai.org/
- A Toronto AI initiative
