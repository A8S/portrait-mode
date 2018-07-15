# Portrait Mode
This project implements the portrait mode effect on images using Neural Networks.

## How it works?
Traditionally, the portrait mode effect has been achieved using 2 lenses which detect ojects present in the foreground and in the background.
With advances in the field of ML, this effect can also be implemented using only image segmentation. Using the pretrained [DeepLab-v3+](https://github.com/tensorflow/models/tree/master/research/deeplab) open source model, we can find the objects in the foreground of the image and blur the background to replicate this effect.

Check out the demo website - [http://portraitmode.herokuapp.com/](http://portraitmode.herokuapp.com/)

## Setup
This project relies on a handful of dependencies, use the following command to install your dependencies:

```shell
pip install -r requirements.txt
```

_Note_: Depending on your environment, you may need to use `sudo`. You may also want to use virtualenv.

## Usage

Portrait Mode Effect is used from the command line:

```shell
python portrait-mode.py -i samples/input-1.jpg
```

`-i/--image`: specifies the image file.

The script outputs one image in the same directory with the name: `input-1-portrait.jpg` 

## Examples

```shell
python3 person_blocker.py -i images/img1.jpg
```

![img1](samples/input-1-portrait.jpg)

```shell
python3 person_blocker.py -i images/img2.jpg -c '#c0392b' -o 'giraffe'
```

![img2](samples/input-2-portrait.jpg)

## To Do
- [ ] Develop API.
- [ ] Develop website.

## Contributions
All patches are welcome!

## License
MIT License - see the [LICENSE](https://github.com/mayank26saxena/portrait-mode/blob/master/LICENSE) file for details.

## Credits
1) [https://ai.googleblog.com/2018/03/semantic-image-segmentation-with.html](https://ai.googleblog.com/2018/03/semantic-image-segmentation-with.html)
2) [https://github.com/tensorflow/models/tree/master/research/deeplab](https://github.com/tensorflow/models/tree/master/research/deeplab)
3) [https://github.com/minimaxir/person-blocker](https://github.com/minimaxir/person-blocker)
