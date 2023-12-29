# gitlab-estudos
Configuração, deployment e teste do gitlab e seus componentes

utilizado:

1 - postgres, redis e minio para storages
2 - 3 vms ubuntu 22.04 para as instâncias gitaly
3 - deployment de um praefect para as 3 instâncias gitaly
4 - helm chart do gitlab personalizado 
5 - helm chart do gitlab-runner para CI 
6 - ingress-nginx para acesso externo do cluster k8s

instruções:
Em cada diretório há um readme com links de referências e explicando os passos a seguir junto com exemplos.
Há também este link para o diagrama do projeto: https://app.diagrams.net/#G1__kT9dsZ25jSUqXB2d2zWNd3AcRIgWR4