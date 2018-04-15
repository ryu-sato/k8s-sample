# k8s-sample

Kubernetes のサンプル集です。

# サンプルについて

k8s 理解のためのものであり、動作を保証するものではありません。

# 使い方

1. GKE のプロジェクトを作成する
1. GKE でクラスタを作成する
1. GKE クラスタの confidential を取得する (kubectl が使えるようになる)
    1. クラスタ一覧を表示する
        `gcloud container clusters list`
    1. クラスタの kubectl 用設定を取得する
        `gcloud container clusters get-credentials ${CLUSTER_NAME}`
1. k8s に deployment, service, ingress を作成する
    `kubectl create -f ${OBJECT-DEF}.yaml`
    - OBJECT-DEF.yaml は deployment/nginx.yaml 等のオブジェクトを定義した YAML ファイルを指定する。

# 備考

- GKE は Node の稼働時間で課金される
