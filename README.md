# helm-charts
[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

helm repo add  https://.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
` to see the charts.

To add the  chart:

    helm repo add lisot https://n-lisot.github.io/helm-charts/

To install the  chart:

    helm install deno-webserver lisot/deno-webserver

To uninstall the chart:

    helm delete deno-webserver
    
    
Changelog
deno-webserver:


0.3.0

    Add InitContainers 
    
    Add Readiness probe to maria db
    
    Add Liveness probe to webserver

0.2.0

    Use release variable to create deploy
    
    Add GitHub action to create release
    
    Add GitPage
    
    Change MariaDB to StatefulSet

0.1.0

    Create helm chart
    
    Create deno-webserver
    
    Create mariadb
