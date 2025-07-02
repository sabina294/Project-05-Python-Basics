# Python Setup

### 1. Install Python 3.13.5 from Source

Python is a high-level, interpreted programming language used to build all kinds of software — from simple scripts to complex web applications and data analysis tools.
The current version I am using is python `v3.13.5`. To install or update to the latest version, open your preferred terminal and run the following commands:

```sh
sudo apt update
sudo apt install python3 -y

```
#### Install required dependencies
```sh
sudo apt update
sudo apt install -y build-essential libssl-dev zlib1g-dev \
  libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev \
  libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev \
  tk-dev libffi-dev curl

```
#### Download and extract Python 3.13.5
```sh
cd /usr/src
sudo curl -O https://www.python.org/ftp/python/3.13.5/Python-3.13.5.tgz
sudo tar xzf Python-3.13.5.tgz
cd Python-3.13.5

```
#### Set Python 3.13.5 as default python3 (optional)
```sh
sudo update-alternatives --install /usr/bin/python3 python3 /usr/local/bin/python3.13 1
sudo update-alternatives --config python3

```

#### Verify
```sh
python3 --version
Output: Python 3.13.5
```

### 2. Install PyCharm

PyCharm is a powerful Integrated Development Environment (IDE) specifically designed for programming in Python. Developed by JetBrains, PyCharm provides a complete toolkit for writing, testing, and debugging Python code efficiently and professionally.
The current version I am using is PyCharm `2025.1`. To install or update to the latest version, open your preferred terminal and run the following commands:

```sh
sudo apt update
sudo apt install snapd

```
####  Install PyCharm (choose one):

```sh
sudo snap install pycharm-community --classic

```

####  Launch PyCharm
```sh
pycharm-community
```

####  Some Plugins Add:
```sh
# Go to pycharm setting>Plugins
.env files support
Atom Material Icon
Git Tool Box
Highlight Bracket Pair
Material Theme
Lines Sorter
Power Shell


```



