# Step of create work enviromental

## 開発

### テンプレートから作成後に実行する

workspace名の変更

    git mv wsXXX.code-workspace wsDST.code-workspace

README.mdのタイトルを変更する

### 環境準備

仮想環境を作成する

    pipenv --python 3.10

uvの方が早い

    uv venv --python 3.13

## UVによる環境作成

### 新規作成

適当なフォルダにて以下でプロジェクトを作成する

    uv init <プロジェクト名> -p <Pythonバージョン>

パッケージを追加する場合は以下

    uv add <パッケージ名>

バージョン指定が必要なら以下

    uv add "<パッケージ名>==<バージョン>"

パッケージを取り除くなら以下

    uv remove <パッケージ名>

### 作成済み環境の同期

pyproject.tomlの存在するフォルダ内で以下コマンドを実行する

    uv sync