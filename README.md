# sample-open-web-ui

このプロジェクトは、Docker Compose を使って Ollama と Open WebUI を Docker コンテナとして起動します。Webインターフェース付きのローカル LLM 環境を簡単に構築できます。

## セットアップ

1. 永続データ用のディレクトリを作成します。

    ```sh
    mkdir -p data/ollama data/open-webui
    ```

2. コンテナを起動します。

    ```sh
    docker-compose up -d
    ```

3. Docker コンテナ内に LLM（gemma4:e4b）をインストールします。

    ```sh
    docker exec ollama ollama pull gemma4:e4b
    ```

4. [http://localhost:3000/](http://localhost:3000/) にアクセスします。

5. 管理者アカウントを新規登録します。
