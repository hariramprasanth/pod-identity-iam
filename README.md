# Pod Identity 
Alpine images has been used for the example since it is light weight. It does not have aws cli pre installed.

To install AWS CLI
1. First ssh into pod via 
`kubectl exec <pod-name> -it -n <namespace> -- /bin/sh`

2. Run the following command
`apk add --no-cache aws-cli`

3. Make sure aws cli installed 
`aws --version`

4. To list the dynamodb tables
`aws dynamodb list-tables`

