# nvim-plugin

## Install neovim
Import Neovim stable PPA: `sudo add-apt-repository ppa:neovim-ppa/stable -y`

Import Neovim unstable PPA: `sudo add-apt-repository ppa:neovim-ppa/unstable -y`

Next, update your package index to include the newly added PPA: `sudo apt update`

Now, you can proceed to install Neovim using the following command: `sudo apt install neovim`

Upon completion, Neovim will be installed on your system using the Neovim Team PPA. You can also verify that the PPA version is installed by running the following command: `apt-cache policy neovim`

## Install Plugins

path: `~/.config/nvim/init.vim`

create folders `.config` and `nvim`

`git clone git@github.com:pandamy619/nvim-plugin.git` to `~/.config/nvim/`\

copy plugin file: `cp nvim-plugin/init.vim ./init.vim`

delete clone directory: `rm -rf nvim-plugin`

install the vim-plug plugin manager: `curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim`

install nvim plugins: 
```bash
nvim
:PlugInstall
:UpdateRemotePlugins
:q!
```
