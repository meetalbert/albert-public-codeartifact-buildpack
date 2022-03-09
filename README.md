# albert-public-codeartifact-buildpack
Heroku buildpack to allow AWS Codeartifact as a pip EXTRA_INDEX_URL

## Required Variables
```
AWS_CODEARTIFACT_ACCESS_KEY_ID
AWS_CODEARTIFACT_SECRET_ACCESS_KEY
AWS_CODEARTIFACT_GET_AUTHORIZATION_TOKEN_ARGS
AWS_CODEARTIFACT_URL
```

- `AWS_CODEARTIFACT_ACCESS_KEY_ID` is the acccess key id for the IAM Role with access to the CodeArtifact instance
- `AWS_CODEARTIFACT_SECRET_ACCESS_KEY` is the secret access key for the IAM Role with access to the CodeArtifact instance
- `AWS_CODEARTIFACT_GET_AUTHORIZATION_TOKEN_ARGS` is the list of arguments to tehe aws command ex: `--domain <DOMAIN> --domain-owner <ACCOUNTID> --query authorizationToken --output text --region <REGION>`
- `AWS_CODEARTIFACT_URL` is the CodeArtifact url ex: `<DOMAIN>-<ACCOUNTID>.d.codeartifact.<REGION>.amazonaws.com/pypi/pypi/simple/`