# .dotfiles

For getting up to speed quickly on a machine

## Bootstrapping a new Macbook

1. Install xcode

    ```bash
    xcode-select --install
    ```

1. Clone this repo however you want

    ```bash
    git clone https://github.com/jbevan4/.dotfiles.git
    ```

1. Install homebrew

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

1. Install all the packages

    ```bash
    brew bundle --file .dotfiles/Brewfile
    ```

1. Install oh-my-zsh

    ```bash
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```

1. Symlink the files

    ```bash
    ln -s .dotfiles/.zshrc .zshrc
    ln -s .dotfiles/.gitconfig .gitconfig
    ```

    1. for the .zshrc mentioned here, you will need to also install [these](https://github.com/powerline/fonts) fonts
    1. Navigate to iterm and update the profile text to mono ubuntu
    1. Update the terminal colours to dark-solarized

1. Install [docker](https://www.docker.com/get-started)

Everything should hopefully now work upon booting up a terminal!

## Security

Replace the key in .gitconfig with one from your machine and update it on github

## TODO

* Find better solution for terminal profile and fonts
