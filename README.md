# Fujitsu Enterprise Postgres Operator Helm Chart description

This Helm Chart makes it easy to deploy Fujitsu Enterprise Postgres Operators in a Kubernetes environment.

# How to deploy the FEP Operator

```
    # helm repo add fep-repo https://fujitsu.github.io/fep-operator-helm/v1
    # kubectl create namespace fep-operator
    # helm install fep-operator-release fep-repo/fujitsu-enterprise-postgres-operator --namespace fep-operator
```

# About clients

Fujitsu Enterprise Postgres clients can be downloaded from the [Fujitsu Enterprise Postgres client - download](https://www.postgresql.fastware.com/fujitsu-enterprise-postgres-client-download) page.

For details on how to install the client, refer to the [Installation and Setup Guide for Client](https://fast.fujitsu.com/hubfs/_Global/Manuals/Anch/InstallationAndSetupGuideForClient.pdf) manual.

# License information

Please note that the Fujitsu Enterprise Postgres Operator installed with this Helm Chart must be purchased and use a product license.
