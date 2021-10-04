# Setup Your Development Environment

Recommended Tools:

* Text Editor
* Terminal
* Package Manager
* ZShell

## MacOS

### Text Editor

Download and install 1 of the following:

* [Atom](https://atom.io/)
* [Sublime Text](https://www.sublimetext.com/)
* [VS Code](https://code.visualstudio.com/)

### Terminal

* [Download and install iterm2](https://iterm2.com/)

### Package Manager (homebrew) and ZShell (zsh)

* Open iterm2

* Install Dev Tools
```bash
sudo xcode-select --install

softwareupdate --all --install --force
```

* Check MacBook Chip
```bash
open -a "About This Mac"
```

    !!! IMPORTANT
        If your chip is "M1", run the following:
        ```bash
        softwareupdate --install-rosetta

        cd && sudo mkdir /opt/homebrew && sudo curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C /opt/homebrew

        arch --x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

        alias brow='arch --x86_64 /usr/local/Homebrew/bin/brew'

        PATH=/opt/homebrew/bin:$PATH

        brew update

        brew doctor
        ```

* Install Homebrew (ONLY IF CHIP IS NOT "M1")
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew update

brew doctor
```

* Install zsh
```bash
brew install zsh

chsh -s /usr/local/bin/zsh
```

    !!! HELP
        If you run into issues, refer to [Installing Zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)

* Download and Install oh-my-zsh
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

    !!! HELP
        If you run into issues, refer to [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)

* Configure Zsh
```zsh
echo "export PATH=''" >> ~/.zshrc

echo path+=('/usr/local/bin') >> ~/.zshrc

echo path+=('/usr/bin') >> ~/.zshrc

echo path+=('/usr/sbin') >> ~/.zshrc

echo path+=('/bin') >> ~/.zshrc

echo "alias bzsh='cp ~/.zshrc ~/.zshrc.bak'" >> ~/.zshrc

echo "alias rzsh='cp ~/.zshrc.bak ~/.zshrc'" >> ~/.zshrc

echo "alias brow='arch --x86_64 /usr/local/Homebrew/bin/brew'" >> ~/.zshrc

echo "path=('/opt/homebrew/bin' $path)"" >> ~/.zshrc

source ~/.zshrc

bzsh
```

## WSL (Windows) - Ubuntu 21.04

* [Install WSL](https://docs.microsoft.com/en-us/windows/wsl/setup/environment)

### Text Editor

Download and install 1 of the following:

* [Atom](https://atom.io/)
* [Sublime Text](https://www.sublimetext.com/)
* [VS Code](https://code.visualstudio.com/)

### ZShell (zsh)

* Install zsh
```bash
sudo apt-get update && sudo apt-get upgrade

sudo apt install zsh

chsh -s $(which zsh)
```

    !!! HELP
        If you run into issues, refer to [Installing Zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)

* Download and Install oh-my-zsh
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

    !!! HELP
        If you run into issues, refer to [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)

* Configure Zsh
```zsh
echo "export PATH=''" >> ~/.zshrc

echo path+=('/usr/local/bin') >> ~/.zshrc

echo path+=('/usr/bin') >> ~/.zshrc

echo path+=('/usr/sbin') >> ~/.zshrc

echo path+=('/bin') >> ~/.zshrc

echo "alias bzsh='cp ~/.zshrc ~/.zshrc.bak'" >> ~/.zshrc

echo "alias rzsh='cp ~/.zshrc.bak ~/.zshrc'" >> ~/.zshrc

echo "alias brow='arch --x86_64 /usr/local/Homebrew/bin/brew'" >> ~/.zshrc

echo "path=('/opt/homebrew/bin' $path)"" >> ~/.zshrc

source ~/.zshrc

bzsh
```
