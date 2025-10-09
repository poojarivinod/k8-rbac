# RBAC

search in google as eks ingress controller--> click on github.io--> Deployment--> Installation Guide

REGION_CODE=us-east-1
CLUSTER_NAME=expense
ACC_ID=695862934667(aws account id)

### Permissions

* OIDC provider
It is authentication service to connect the aws and expense cluster(kubernates)

```
eksctl utils associate-iam-oidc-provider \
    --region $REGION_CODE \
    --cluster $CLUSTER_NAME \
    --approve
```