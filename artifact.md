# Artifact
In general software terms, an "artifact" is something produced by the software development process, whether it be software related documentation or an executable file.

### Name:
It defines the artifact name.

## Repository

### Repository URL:
It defines the repository url for where pick up the sources. Note: we support nexus repository.

### Repository Name:
It defines the repository name inside the nexus repository.

## Authentication

### Username:
It defines the username for nexus repository.

### Password:
It defines the password for nexus repository.

## Artifact

### Identifier:
It defines the location of the package to download. It can be URL,S3,local path or maven identifier

### Version:
It defines the version of the artifact file.

### Checksum:
This checksum is used for whether package properly download or not.

### Path:
This path defines the location of the package inside the nexus repository.

## Destination

### Install directory:
It defines the installation directory of the package.

### Deploy as user:
This user defines, package is deployed by the user what you given in user name.

### Deploy as group:
This group defines, package is deployed by the user what you given in user name.

### Environment variables:
Specify the variables, it will be available on the deployment.

### Persistent directory:
It defines the list of Persist directory. It used for when code is updated, the persist directory does not affect.

### Expand:
It is checked then downloaded package is extracted and placed in specified path in install Directory.

## Stages:

### Configure:
It defines, the command is executed before Configuring the artifact package.

### Migrate:
It defines, the command is executed during migrating stage.

### Restart:
It defines, the command is executed on Restart.
**Ex.**
```
If you want deploy the web application, copy the package into the webapp directory on VM restart.
```
