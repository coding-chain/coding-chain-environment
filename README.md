# Environment

#Pull submodules
To get functional environment you have to clone git submodules of the project.
```shell
git submodule update --init --recursive     
```

## Run local environment
To build and run local environment run this command:
```shell
docker-compose  -f docker/docker-compose.yml  up
```

## Generate certificate on Windows

```
dotnet dev-certs https -ep docker/neos-coding-api/CodingChainApi.WebApi.pfx -p { password here }
dotnet dev-certs https --trust
```

## Generate certificate on  macOs or Linux

```
dotnet dev-certs https -ep ${HOME}/.aspnet/https/CodingChainApi.WebApi.pfx -p { password here }
dotnet dev-certs https --trust
```
