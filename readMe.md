# AEM Developer Stack

This [docker-compose](https://docs.docker.com/compose/) script allows a full Adobe Experience Manager (AEM)
6 stack to be deployed within a Docker container.

**NOTE:** You must have a copy of the AEM 6 installation media for this to work!

## Usage
Copy your the installation media and license files into the author and publisher directories.
The install media must be given specific names depending on location. `cq-author-4502.jar` for author, and `cq-publish-4503.jar` for the publisher. It should appear as follows:

```
.
|-- docker-compose.yml
|-- readMe.md
|-- publisher
|   |-- Dockerfile
|   |-- cq-publish-4503.jar [User Added]
|   `-- license.propeties [User Added]
`-- author
    |-- Dockerfile
    |-- cq-author-4502.jar [User Added]
    `-- license.propeties [User Added]
```

Enter the following to start the environment
```bash
docker-compose up
```
