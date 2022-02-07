# FUJITSU Enterprise Postgres Operator Helm Chart description

This Helm Chart makes it easy to deploy FUJITSU Enterprise Postgres Operators in a Kubernetes environment.

# How to deploy the FEP Operator

```
    # helm repo add fep-repo https://fujitsu.github.io/fep-operator-helm/v1
    # kubectl create namespace fep-operator
    # helm install fep-operator-release fep-repo/fujitsu-enterprise-postgres-for-kubernetes-namespace fep-operator
```

# How to upgrade an FEP Operator

Helm does not support the upgrade of CRDs, and must be manually updated prior to the upgrade.

```
    # helm repo update
    # helm search repo fujitsu-enterprise-postgres-for-kubernetes
    # helm show crds fep-repo/fujitsu-enterprise-postgres-for-kubernetes > crds.yaml
    # kubectl apply -f crds.yaml
    # helm upgrade fep-operator-release fep-repo/fujitsu-enterprise-postgres-for-kubernetes-namespace fep-operator
```

# About clients

FUJITSU Enterprise Postgres clients can be downloaded from the [FUJITSU Enterprise Postgres client - download](https://www.postgresql.fastware.com/fujitsu-enterprise-postgres-client-download) page.

For details on how to install the client, refer to the [Installation and Setup Guide for Client](https://fast.fujitsu.com/hubfs/_Global/Manuals/Anch/InstallationAndSetupGuideForClient.pdf) manual.

# License information

Please note that the FUJITSU Enterprise Postgres Operator installed with this Helm Chart must be purchased and use a product license.
