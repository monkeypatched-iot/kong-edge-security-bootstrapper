# security-bootstrapper


the security bootstrapper extend the base commands provided by the edgex security bootstrapper and allows the commands to be executed to generate internal passwords and secure connections to http and tcp connections liveness and wait for services to connect 

inorder to test the docker container first execute 

``` sudo docker ps ```

this should give you the id of the container and then run the commands for the bootstrapper as shown below 

``` sudo docker exec -it <ContainerID> ./security-bootstrapper help ``` 

the complete list of commands can be found below 

```
Usage: ./security-bootstrapper [options] <command> [arg...]
Options:
    -h, --help    Show this message
    --configDir     Specify local configuration directory

Commands:
    gate              Do security bootstrapper gating on stages while starting services
    genPassword       Generate a random password
    getHttpStatus     Do an HTTP GET call to get the status code
    help              Show available commands (this text)
    listenTcp         Start up a TCP listener
    setupRegistryACL  Set up registry's ACL and configure the access
    waitFor           Wait for the other services with specified URI(s) to connect:
                      the URI(s) can be communication protocols like tcp/tcp4/tcp6/http/https or files

```

