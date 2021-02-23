helm install my-pg-auth -f postgres-auth.yaml bitnami/postgresql

helm install my-pg-serv -f postgres-serv.yaml bitnami/postgresql


helm install my-auth -f otus-sample-auth.yaml ./otus-sample-auth

helm install my-serv -f otus-sample-serv.yaml ./otus-sample-serv

helm install my-ing1 -f otus-sample-ing.yaml ./otus-sample-ing1

helm install my-ing2 -f otus-sample-ing.yaml ./otus-sample-ing2

helm uninstall my-ing1

helm uninstall my-ing2

helm uninstall my-serv

helm uninstall my-auth

helm uninstall my-pg-serv

helm uninstall my-pg-auth