# Unix Config

This repo should contains all configs associated with unix systems to help daily drive.

Each branch should represent a specific environment, master being the most general, applicable for a new config from sratch.

## FIRST ! Install zsh and ohmyzsh and copy .zshrc

```
apt install zsh curl
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## ALL Dependencies needed

First : `sudo apt update && upgrade`

### All dependencies for Normal Nvim
```bash
sudo apt update; sudo apt install --install-if-missing "luarocks" "yarn" "rust-fd-find" "python-pytest" "delta" "rust-grcov" "rustup" "gcc-defaults" "binutils" "dotnet8" "monodevelop" "java-common" "nasm" "r-base" "rustc" "golang" "python" "ruby" "perl" "lua5.3" "kotlin" "elixir" "make" "nodejs" "npm" "node-typescript" "nuitka" "doxygen" "yard"; pip install "pyinstaller"; yarn global add "jest" "jsdoc" "typedoc"; cargo install "yazi-fm"; go install "golang.org/x/tools/cmd/godoc@latest"; sudo snap install --classic "flutter"
```


### Cool utilitaries
```ranger tilix neofetch google-chrome-stable```

### node

Checkout and follow : https://github.com/nvm-sh/nvm

```bash
nvm install --lts && nvm use --lts
```



## Neovim

To install neovim, the prefered way is to compile it from source.

Git clone the repo, go to the prefered branch then :
```bash
make CMAKE_BUILD_TYPE=RelWithDebInfo
sudo make install
```

It should be installed globally.


Then goto ~/.config and git clone my repo normal nvim :
```bash
git clone git@github.com:AronGomu/Normal_Nvim_AronGomu.git nvim
```

It has to be named nvim to be functionnal.
