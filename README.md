# Example Mac dev environment with zsh, oh-my-zsh, pyenv with python 3.7 & anaconda


1. install homebrew  `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`
2. install zsh `brew install zsh`
3. install oh-my-zsh `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
4. ensure zsh is default bash
5. `brew install coreutils`
6. install pyenv (python version manager) by following these instructions https://github.com/pyenv/pyenv#basic-github-checkout
7. installing anaconda `brew cask install anaconda`
8. conda won't work until .zsh has conda added to the path, `conda init zsh` does this but needs to be run from conda's executable (because conda not in path) `/usr/local/anaconda3/bin/conda init zsh`
9. Disable the base environment for conda `conda config --set auto_activate_base false`
Note: not recomended to run base anaconda anvironment as per SO answers below.


https://brew.sh/

https://stackoverflow.com/questions/58044214/installing-anaconda-with-pyenv-unable-to-configure-virtual-environment
https://stackoverflow.com/questions/57640272/how-can-i-install-anaconda-aside-an-existing-pyenv-installation-on-osx
https://www.anaconda.com/blog/using-pip-in-a-conda-environment


Specific pitfalls: 
