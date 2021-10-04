# go-web-server

## Deployment

### Dockerfile
Enter `$ ./ci/deploy-dockerfile.sh` on the terminal to build image and deploy server with docker build and run commands

### Docker compose
Enter `$ ./ci/deploy-docker-compose.sh` on the terminal to build image and deploy server with docker build and run commands

### Testing server locally
Testing endpoints below show display the messages below
1. http://localhost:8081/hello - displays `188: responding from the go-web-server`
2. http://localhost:8081/health - displays `153: ok`
3. http://localhost:8081/keyword - displays `153: wellness`
4. http://localhost:8081/ - displays `404`
 