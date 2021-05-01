# Api

Generate certificate :

## On Windows

```
dotnet dev-certs https -ep docker/neos-coding-api/CodingChainApi.WebApi.pfx -p { password here }
dotnet dev-certs https --trust
```

## On macOs or Linux

```
dotnet dev-certs https -ep ${HOME}/.aspnet/https/CodingChainApi.WebApi.pfx -p { password here }
dotnet dev-certs https --trust
```
