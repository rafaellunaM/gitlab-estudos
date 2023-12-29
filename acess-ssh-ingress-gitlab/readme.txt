Precisa adicionar no deployment do nginx:
args:
  - /nginx-ingress-controller
  - --tcp-services-configmap=gitlab/tcp-configmap-example


referencia: https://docs.gitlab.com/charts/advanced/external-nginx/
