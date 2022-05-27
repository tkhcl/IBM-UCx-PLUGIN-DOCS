
Docker Build - Documentation
============================

# Overview




### Overview




 


Docker is an open platform for distributed applications for developers and sysadmins.  

Leverage
 this plugin to build Docker images with UrbanCode Build


The Docker plug-in includes the following steps that are 
related to Docker:


* [Docker Build](steps/#docker_build "docker_build")
* [Docker Push](steps/#docker_push 
"docker_push")


To add the Docker plug-in steps to processes, click **Build > Build Tools > Docker** when adding new 
steps to a job.


### Compatibility


The IBM UrbanCode Build plug-in for Docker works with all versions of Docker



This plug-in requires version 6.1.0.0 or later of IBM UrbanCode Build.


### Installation


No special steps are 
required for installation.


### History


#### Version 2


Version 2 supports IBM UrbanCode Build version 6.1.0.0. The 
following features were added:


* Added a step to push Docker images to a registry.


#### Version 1


Version 1 
supports IBM UrbanCode Build version 6.1.0.0.


* Initial release supporting building Docker images


# Steps




### Steps




 



### Job steps in the Docker plug-in


* [Docker Build](#docker_build)
* [Docker 
Push](#docker_build)




### Docker Build


Build a Docker image from a Dockerfile and set the image id as a build life 
property.




*Input properties for the  

Docker Build step*  | Name | Type | Description | Required |
| --- | --- | 
--- | --- |
| Image Property | String | The name of the build life property to set the image id as. | No |
| 
DOCKER\_HOST | String | Optionally use a different Docker host value than the default. e.g. tcp://host:port | No |
| Tag
 | String | The name to tag the image with if the build is successful. | No |
| Build Flags | String | Additional flags 
to pass to Docker build. e.g. no-cache=true -q rm=true | No |


### Docker Push


Publish a Docker image to a registry.





*Input properties for the  

Docker Push step*  | Name | Type | Description | Required |
| --- | --- | --- | --- |

| DOCKER\_HOST | String | Optionally use a different Docker host value than the default. e.g. tcp://host:port | No |
| 
Image Name | String | The name of the image to push to the registry. e.g. username/ubuntu or 
localhost.localdomain:5000/ubuntu | Yes |
| Username | String | The username used to log in to the registry | Yes |
| 
Password | String | The password used to log in to the registry | Yes |
| Email | String | The email address used to log
 in to the registry | Yes |
| Server | String | The registry server. e.g. localhost:5000. If no server is specified, 
https://index.docker.io/v1 is the default. | No |




