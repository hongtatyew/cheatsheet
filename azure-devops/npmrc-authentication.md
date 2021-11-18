# Authenticate your local repository to connect to Azure DevOps artifect

```powershell
npm install -g vsts-npm-auth
vsts-npm-auth -config .npmrc -targetconfig c:/users/<username>/.npmrc -v detailed -f

or 

npx vsts-npm-auth -config .npmrc -targetconfig c:/users/<username>/.npmrc -v detailed -f
```