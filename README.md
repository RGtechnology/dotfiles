# dotfiles

Welcome to my dotfiles repository!

## Introduction

This repository contains configuration files and scripts to set up my environment quickly and consistently across different machines.


## Installation macOS

To install these dotfiles, follow these steps:

1. **Clone the repository:**

    ```sh
    git clone https://github.com/RGtechnology/dotfiles.git
    cd dotfiles
    ```

1. **Install GNU Stow**
    
    GNU Stow is a symlink farm manager, which means it helps you store all your configuration files in one common location. So when you "stow" a file, it will create a symlink between your file and an identical file in our home directory. 

    ```sh
    brew install stow
    ```    

1. **Create Symlinks**

    Simulate stow
    ```sh
    cd ~/dotfiles
    stow . -vv --simulate
    ```
    Execute stow
    ```sh
    cd ~/dotfiles
    stow . -vv
    ```

## Usage

After installation, your environment will be configured with the settings from these dotfiles. You can customize them further by editing the files directly. Don't forget to commit the changes in the Git repository.

## Customization

- `.zshrc` - Configuration for Zsh shell
- `.gitconfig` - Configuration for Git
- `.config/starship.toml` - Configuration for Starship prompt

## Contributing

If you have suggestions or improvements, feel free to open an issue or submit a pull request. Contributions are welcome!

## License

This repository is licensed under the MIT License. See the LICENSE file for more details.