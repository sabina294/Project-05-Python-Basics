# Python Environment Setup Guide

This guide walks you through setting up Python 3.13.5 and PyCharm (2025.1) on a Linux system, optimized for development and productivity.

---

## 🐍 Python 3.13.5 Setup

Python is a high-level, interpreted language widely used for scripting, data science, automation, and web development.

### ✅ Prerequisites

Before installing Python, make sure your system is updated and has the necessary build dependencies:

```bash
sudo apt update
sudo apt install -y build-essential libssl-dev zlib1g-dev \
  libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev \
  libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev \
  tk-dev libffi-dev curl
📥 Download and Compile Python 3.13.5
bash
Copy
Edit
cd /usr/src
sudo curl -O https://www.python.org/ftp/python/3.13.5/Python-3.13.5.tgz
sudo tar xzf Python-3.13.5.tgz
cd Python-3.13.5
./configure --enable-optimizations
make -j$(nproc)
sudo make altinstall
🧭 Set Python 3.13.5 as Default (Optional)
bash
Copy
Edit
sudo update-alternatives --install /usr/bin/python3 python3 /usr/local/bin/python3.13 1
sudo update-alternatives --config python3
🔍 Verify Installation
bash
Copy
Edit
python3 --version
# Output: Python 3.13.5
🛠 PyCharm 2025.1 Installation
PyCharm is a feature-rich IDE built for Python development. We’ll install the Community Edition via Snap.

📦 Install Snap (if not installed)
bash
Copy
Edit
sudo apt update
sudo apt install snapd
💻 Install PyCharm Community Edition
bash
Copy
Edit
sudo snap install pycharm-community --classic
🚀 Launch PyCharm
bash
Copy
Edit
pycharm-community
⚙ Recommended PyCharm Plugins
To boost your development experience, consider installing the following plugins:

.env files support – Readable environment variable files.

Atom Material Icons – Enhanced file explorer icons.

Git ToolBox – Advanced Git features.

Highlight Bracket Pair – Easy navigation through nested code.

Material Theme UI – Beautiful themes for PyCharm.

Lines Sorter – Quickly sort lines in a file.

PowerShell – PowerShell support if working cross-platform.
