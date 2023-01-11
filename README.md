# Dev-Environment
Dev Environment Setup

## Setup Python using [pyenv](https://github.com/pyenv/pyenv)
1. remove previously installed python `sudo apt-get -y purge python3.8` && `sudo apt-get -y autoremove`
2. `sudo apt-get update`
3. 
    ```
    sudo apt install \
        build-essential \
        curl \
        libbz2-dev \
        libffi-dev \
        liblzma-dev \
        libncursesw5-dev \
        libreadline-dev \
        libsqlite3-dev \
        libssl-dev \
        libxml2-dev \
        libxmlsec1-dev \
        llvm \
        make \
        tk-dev \
        wget \
        xz-utils \
        zlib1g-dev
    ```
5. `curl https://pyenv.run | bash`
6. `export PATH="$HOME/.pyenv/bin:$PATH" && eval "$(pyenv init --path)" && echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n eval "$(pyenv init -)"\nfi' >> ~/.bashrc`
7. `exec $SHELL`
8. `pyenv install 3.xxxxxx` (see available list using `pyenv install --list`)
9. `pyenv versions`
10. `pyenv global 3.xxxxx`
## Setup [Virtualenv](https://pypi.org/project/virtualenv/)
