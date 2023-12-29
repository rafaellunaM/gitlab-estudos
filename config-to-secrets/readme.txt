initial root password: senha usada para logar na ui feito root, login: root senha: definidas no secret

rails e registry storage usando minio e sao gerados o token pela ui do minio

criar arquios de secret exemplo:
usam base64

kubectl create secret -n gitlab generic gitlab-gitlab-initial-root-password  --from-literal=password=gitlab-gitlab-initial-root-password
kubectl create secret -n gitlab generic gitlab-gitlab-initial-root-password  --from-file=password=gitlab-gitlab-initial-root-password

exemplo de decode dos arquios:

kubectl get secrets -n gitlab gitlab-gitlab-initial-root-password -o jsonpath='{.data.password}' | base64 -d
kubectl get secrets -n gitlab  gitlab-runner -o jsonpath='{.data.runner-registration-token}' | base64 -d


link de exemplo dos storages:
https://gitlab.com/gitlab-org/charts/gitlab/-/tree/master/examples/objectstorage