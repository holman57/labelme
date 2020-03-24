
# Install 

```bash
pip install -e .
```

## Usage

Run `labelme` to start the application
Run `labelme --help` for detail. 

- The first time you run labelme, it will create a config file in `~/.labelmerc`. You can edit this file and the changes will be applied the next time that you launch labelme. If you would prefer to use a config file from another location, you can specify this file with the `--config` flag.

```bash
# Setup conda
conda create --name labelme python==3.6.0
conda activate labelme

# Build the standalone executable
pip install .
pip install pyinstaller
pyinstaller labelme.spec
dist/labelme --version
```

## Acknowledgement

This repo is the fork of [mpitid/pylabelme](https://github.com/mpitid/pylabelme),
whose development has already stopped.

```bash
@misc{labelme2016,
  author =       {Kentaro Wada},
  title =        {{labelme: Image Polygonal Annotation with Python}},
  howpublished = {\url{https://github.com/wkentaro/labelme}},
  year =         {2016}
}
```

B. C. Russell, A. Torralba, K. P. Murphy, W. T. Freeman. LabelMe: a Database and Web-based Tool for Image Annotation. International Journal of Computer Vision, 77(1-3):157-173, 2008. [Project page](http://labelme.csail.mit.edu/Release3.0/)