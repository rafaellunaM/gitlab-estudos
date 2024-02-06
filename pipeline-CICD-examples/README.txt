The idea in this example is to have two repositories in Gitlab

The first sends the commit
The second receives the commit

To do this, a CI/CD pipeline is created in the 'ENVIA-COMMIT-CI' repository
where you use kaniko to build the whoami image defined in the Dockerfile
and named with the SHA short of the image

After the build stage it is passed to the Send stage to the 'RECEBE-COMMIT-CI' repository
where only the image tag written in values ​​is changed.

In this process, argocd, gitlab, helm and k8s are used