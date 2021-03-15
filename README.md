# Variety-Windows

Variety-Windows is Windows port of [Variety](https://github.com/varietywalls/variety),
which is a wallpaper manager. It supports numerous desktops
and wallpaper sources, including local files and online services: Flickr,
Wallhaven, Unsplash, and more.

Where supported, Variety sits as a tray icon to allow easy pausing and resuming.
Otherwise, its desktop entry menu provides a similar set of options.

Variety also includes a range of image effects, such as oil painting and blur,
as well as options to layer quotes and a clock onto the background.

## Installation

### Install from source
To install Variety from source, you will need Git, Python 3.5+ and [distutils-extra](https://launchpad.net/python-distutils-extra). To actually run Variety, you will also need the following:

#### Runtime Requirements
- GTK+ 3
- gexiv2
- libnotify
- Python 3 libraries:
    - BeautifulSoup4
    - lxml
    - Pycairo
    - PyGObject, built with Cairo integration
    - ConfigObj
    - Pillow
    - pkg_resources (from setuptools)
    - Requests
    - *Optional*: httplib2 (for more quotes sources)
- *Optional*: imagemagick (for wallpaper filters)

#### Install steps

1. Clone the git repository: `git clone https://github.com/varietywalls/variety.git && cd variety`

2. Run `python3 setup.py install`. By default, this will install Variety into `/usr/local`; for a local installation, use `python3 setup.py install --prefix $HOME/.local`.

3. Run `variety` from the command line or its desktop menu entry!
