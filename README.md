# ダミー会社サイト - GitHub Pages 公開手順

## フォルダ構成
```
dummy-sites/
├── index.html          ← 管理用トップページ（このファイル）
├── towa-kinzoku/       ← 東和金属工業
│   └── index.html
├── sanei-plastic/      ← 三栄プラスチック製造
│   └── index.html
├── hokuriku-seimitsu/  ← 北陸精密機器
│   └── index.html
├── shinko-denshi/      ← 新興電子部品工業
│   └── index.html
└── taiyo-gomu/         ← 大洋ゴム化工品
    └── index.html
```

## GitHub Pages 公開手順

### 1. GitHubで新しいリポジトリを作成
- リポジトリ名: `dummy-sites`（非公開にしたい場合はPrivateでもOK）
- ※GitHub Pagesは**Publicリポジトリ**なら無料

### 2. ファイルをアップロード
方法A（簡単）: GitHubのWebサイトからドラッグ＆ドロップ
方法B: Git CLIを使う場合
```bash
git init
git add .
git commit -m "add dummy sites"
git remote add origin https://github.com/【ユーザー名】/dummy-sites.git
git push -u origin main
```

### 3. GitHub Pagesを有効化
1. リポジトリの「Settings」を開く
2. 左メニュー「Pages」をクリック
3. Source: 「Deploy from a branch」を選択
4. Branch: `main` / `/(root)` を選択して「Save」

### 4. 数分後にURLが発行される
```
https://【ユーザー名】.github.io/dummy-sites/towa-kinzoku/
https://【ユーザー名】.github.io/dummy-sites/sanei-plastic/
https://【ユーザー名】.github.io/dummy-sites/hokuriku-seimitsu/
https://【ユーザー名】.github.io/dummy-sites/shinko-denshi/
https://【ユーザー名】.github.io/dummy-sites/taiyo-gomu/
```

## フリーランサーへの渡し方
上記URLをスプレッドシートのリストに割り当てて渡す。
フォームに送信が来たら → どのダミーサイト経由かで確認できる。
