# background_generator

## generate pretty desktop background with 2D gray codes

### fun facts about the images:
- each colour (i.e. (r, g, b) triple) appears exactly once in each image (yes, in every single one!)
- each pixel differs from its four neighbours by exactly one bit (the Gray property)
- the Gray property is cyclic, so tiling the images creates a flawless periodic pattern

### requirements and configuration

#### requirements

- Linux
- `feh` and `python` (3) installed on your system
- `numpy` installed for python

#### configuration

there is none.

when the program is run, it will use feh to set your background to a freshly generated image. it takes a single positional argument: the time in seconds between refreshing the background with a newly generated image. anything but a positive real (including no argument at all) will turn off automatic image refreshing.

to run on startup, the usual: add it to your path and add a line `.xinitrc`, `profile.sh` or similar. don't forget &

### some random samples:
![24](https://github.com/qdbp/background_generator/blob/master/test_random_24.png)
![27](https://github.com/qdbp/background_generator/blob/master/test_random_27.png)
![95](https://github.com/qdbp/background_generator/blob/master/test_random_95.png)
