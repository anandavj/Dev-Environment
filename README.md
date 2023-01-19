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

## Setup Node using [nvm](https://github.com/nvm-sh/nvm)
1. `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash`
2. `export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"`
3. `nvm install node`

## Setup Golang
1. `curl -OL https://golang.org/dl/go1.18.10.linux-amd64.tar.gz`
2. `sudo tar -C /usr/local -xvf go1.18.10.linux-amd64.tar.gz`
3. `export GOROOT=/usr/local/go`
4. `export GOPATH=$HOME/go`
5. `export PATH=$GOPATH/bin:$GOROOT/bin:$PATH`
6. `source ~/.bashrc`

## Setup [Virtualenv](https://pypi.org/project/virtualenv/)
