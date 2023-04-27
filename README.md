# security-bootstrapper


the security bootstrapper extend the base commands provided by the edgex security bootstrapper and allows the commands to be executed to generate internal passwords and secure connections to http and tcp connections liveness and wait for services to connect 

inorder to do so first execute 

``` sudo docker ps ```

this should give you the id of the container and then run the commands for the bootstrapper as shown below 

``` sudo docker exec -it <ContainerID> ./security-bootstrapper help ``` 
