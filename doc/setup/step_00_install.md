# 開発環境設定
## Docker Desktopのダウンロードとインストール
https://www.docker.com/products/docker-desktop/
## VSCordのダウンロードとインストール
https://code.visualstudio.com/download
- 必要に応じて拡張機能のインストール
## asdf のインストール 
```bash
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.13.1
echo -e '\n. $HOME/.asdf/asdf.sh' >> ~/.bashrc
echo -e '\n. $HOME/.asdf/completions/asdf.bash' >> ~/.bashrc
source ~/.bashrc
```
## erlang + elixir のインストール
```bash
asdf plugin add erlang https://github.com/asdf-vm/asdf-erlang.git
asdf plugin add elixir https://github.com/asdf-vm/asdf-elixir.git
asdf install erlang latest
asdf global erlang latest
asdf install elixir latest
asdf global elixir latest
elixir -v
```
## Phoenixのインストール
```bash
mix archive.install hex phx_new
```
