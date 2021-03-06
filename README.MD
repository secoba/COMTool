COMTool
========

 [![PyPI](https://img.shields.io/pypi/v/comtool.svg)](https://pypi.python.org/pypi/comtool/)

A cross platform serial debug tools written by python
--------

Windows(version 1.0,not the latest)
![Windows screenshot](./COMToolData/assets/screenshot_V1.3.png)
Linux(Elementry OS)
![Linux(Elementry OS)screenshot](./COMToolData/assets/screenshot_V1.4_night.png)
Raspberry Pi3
![Raspberry Pi screenshot](./COMToolData/assets/RaspberryPiScreenshot.png)
> screenshot shows the version 1.0, the latest may not the same totally! But better performance、more easy to use and more elegant

## Features

- [x] cross platform (Windows, Linux, MacOS, Raspberry Pi ... ...)
- [x] port baudrate bytesize parity stopbits settings
- [x] basic send data (ascii and hex)
- [x] basic receive data (ascii and hex)
- [x] send and receive data count
- [x] clear received data area
- [x] auto linefeed on every once receive
- [x] scheduled auto send
- [x] send history and select send again
- [x] serial auto detect
- [x] CR LF / LF select support
- [x] auto save settings
- [x] <kbd>Ctrl+Enter</kbd> to send
- [ ] escape character support, like \x \r \n etc.
- [ ] multiple character encode support
- [ ] multiple auto send (order and disorder)
- [ ] unix style terminal color support
- [x] night theme and White theme
- [ ] real time data graphic display

## Install

### Windows

Test pass on Win10

there's three ways:
1. download excutable bin file, easiest way for one never used python
  * Download the latest bin file at the [release page](https://github.com/Neutree/COMTool/releases)
  * unzip, and run comtool.exe
2. Install Python3 first then install from pypi:
  * [dowload python3](https://www.python.org/downloads/)
  * Install by pip,
```
pip install comtool
comtool
```
3. Or you can download source code, then install from source code
  * download sourcecode
  * install
```
python setup.py bdist_wheel
pip install dist/COMTool-*.*.*-py3-none-any.whl
comtool
```


### Linux

Test on Ubuntu 16 and Elementry OS 4

* download and install
```
sudo apt install python3
sudo apt install python3-pip
sudo pip3 install comtool
sudo comtool
```
or
```
sudo apt install python3
wget https://bootstrap.pypa.io/get-pip.py 
sudo python3 get-pip.py
sudo pip3 install comtool
sudo comtool
```
> be sure python bin path already in the `$PATH` env.



 Or you can download source code, then install from source code
  * download sourcecode
```
python setup.py bdist_wheel
sudo pip3 install dist/COMTool-*.*.*-py3-none-any.whl
```


### macOS

```
brew install python3 python3-pip
pip install COMTool
```

### Rasberry Pi

Test pass on Raspberry Pi 3
just open terminal, type the command below:
```
sudo apt install git
git clone https://github.com/Neutree/COMTool.git
cd COMTool
python setup.py bdist_wheel
sudo pip3 install dist/COMTool-*.*.*-py3-none-any.whl
comtool
```
then enjoy

## Development

1. Install python3.6 and pip3
Linux:
```
sudo apt install python3 python3-pip
```

Windows: 
  [dowload python3](https://www.python.org/downloads/)

2. install pyserial and PyQt5
```
sudo pip install pyserail pyqt5 bs4
```
On Raspberry:
```
sudo pip install --upgrade pyserial bs4
sudo apt install python3-pyqt5
```

3. clone project
```
git clone https://github.com/Neutree/COMTool.git
```

4. code, resolve bugs or add new reatures


5. pull request

## Issue and improvement
create issue [here](https://github.com/Neutree/COMTool/issues/new)



