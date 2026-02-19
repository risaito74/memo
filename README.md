# memo
純粋なメモ書き、特定のリポジトリに依存しないやつ

## 👉Unityプロジェクト（完成済）を GitHub Desktop でリポジトリ化する手順

### 1) 新規リポジトリ作成
GitHub Desktop のメニューから：

- `File` > `New repository...`

### 2) git ignore は Unity を選ぶ（重要）
- `git ignore` は **Unity** を選択する  
- これを入れないと、Unityプロジェクトの巨大ファイル群まで含めて push しようとして **詰む（数GB）**

### 3) Local path の指定に注意（重要）
- Local path は `C:\unity\` のように **プロジェクトフォルダ名を抜いた親フォルダ** を指定する
- GitHub Desktop 側でリポジトリ名が結合されて、最終的にプロジェクトフォルダが作られる

例：

- Local path：`C:\unity\`
- Repository name：`MyUnityProject`

→ 作成される場所：`C:\unity\MyUnityProject`

### 4) 最初の push 時の公開設定
最初にリモートへ上げる時に：

- **Public / Private のチェック**を確認する（意図どおりになってるか見る）
