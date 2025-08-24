# Linux で yazi を使う設定メモ

## Linux / WSL セットアップ
### インストール
#### Debian / Ubuntu 系
```bash
sudo apt update
sudo apt install yazi
```

#### Arch系
```bash
sudo pacman -S yazi
```

#### Homebrew (WSL / Linux 共通)
```bash
brew install yazi
```

### フォント
```bash
# Nerd Font のインストール例
sudo apt install fonts-cascadia-code
# または Nerd Fonts 公式サイトから ttf をダウンロードして ~/.local/share/fonts に置く
fc-cache -fv
```

### プレビュー関連
```
sudo apt install chafa viu
# 画像プレビューが必要なら ueberzugpp も導入
```


