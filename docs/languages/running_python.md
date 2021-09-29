# Running Python

## MacOS

### Install Homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew update

brew doctor
```

### Install Pyenv

```bash
brew install openssl readline sqlite3 xz zlib

brew install pyenv

echo "path=('$HOME/.pyenv/shims' $path)" >> ~/.zshrc

echo "export PATH" >> ~/.zshrc

echo 'eval "$(pyenv init --path)"' >> ~/.zshrc

source ~/.zshrc
```

### Install Python 3

```bash
pyenv install 3.9.6
```

### Create Working Directory

```bash
mkdir practice/python

cd practice/python

pyenv local 3.9.6
```

### Run `test.py`

```bash
echo "print('Test Successful!')" > test.py

python test.py
```
