# serverless-operator

## Operator Install

List all the known tags.
```shell
git tag
```

### Local Install
Clone the remote repository.
```shell
git clone https://github.com/cgfulton/serverless-operator.git
```

Fetch all the known tags.
```shell
git fetch --all --tags
```

Specify the tag and branch to be checkout.
```shell
git chechkout tags/<tag> -b <branch>
```

Install the operator from the local directory.
```shell
oc apply -k .
```

### Remote install
Install the operator from the remote tag.
```shell
oc apply -k https://github.com/cgfulton/serverless-operator.git?ref=<tag-name>
```