# Windows で yazi を使う設定メモ

## 1. フォント (Nerd Font) の導入
1. Nerd Font をダウンロードして解凍  
2. `.ttf` ファイルを右クリック → **インストール** または **すべてのユーザーにインストール**  
3. Windows に登録される

---

## 2. Windows Terminal の設定
- 設定ファイル:
    ```bash
    %LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState\settings.json
    ```
- 開き方: `Ctrl + ,` → 右上の「settings.json を開く」  
- GUI から設定する場合:  
- 設定画面 → プロファイル (PowerShell / Git Bash / WSL) → 外観 → フォントフェイス  
- 例: `CaskaydiaCove Nerd Font`を入れる場合
    ```json
    "profiles": 
    {
        "defaults": {
            "font": {
                "face": "CaskaydiaCove Nerd Font"
            }
        },
        "list": ...
    ```

---

## 3. Git Bash 単独 (mintty) の場合
- Git Bash ウィンドウ → 右クリック → オプション → テキスト → フォント  
- インストール済み Nerd Font を選択

---

## 4. 画像プレビューについて
- Windows ネイティブの PowerShell / CMD では不可  
- Git Bash / WSL 環境なら一部可能 (`ueberzugpp`, `chafa`, `viu`)  
- 画像が不要ならフォント設定だけで十分