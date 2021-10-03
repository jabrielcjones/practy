# Running Python

## MacOS

1. Install Pyenv
```bash
softwareupdate --all --install --force

brew install openssl readline sqlite3 xz zlib

brew install pyenv

echo "path=('$HOME/.pyenv/shims' $path)" >> ~/.zshrc

echo "export PATH" >> ~/.zshrc

echo 'eval "$(pyenv init --path)"' >> ~/.zshrc

source ~/.zshrc
```

1. Install Python 3
```bash
pyenv install 3.9.6
```

1. Create Working Directory
```bash
mkdir practice/python

cd practice/python

pyenv local 3.9.6
```

1. Run `test.py`
```bash
echo "print('Test Successful!')" > test.py

python test.py
```
