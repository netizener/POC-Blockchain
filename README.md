# POC-Blockchain
 ### Setting up the environment :
 1. Run the 'prereqs-ubuntu.sh' file in bash : ./prereqs-ubuntu.sh
 2. Essential CLI tools: 
    npm install -g composer-cli@0.20
 3. Utility for running a REST Server on your machine to expose your business networks as RESTful APIs:
    npm install -g composer-rest-server@0.20
 4. Useful utility for generating application assets:
    npm install -g generator-hyperledger-composer@0.20
 5. Yeoman is a tool for generating applications, which utilises generator-hyperledger-composer:
    npm install -g yo
 6. Install playground : npm install -g composer-playground@0.20
 7. Starting and Stopping Fabric : 
    cd ~/fabric-dev-servers
    export FABRIC_VERSION=hlfv12
    ./startFabric.sh
    ./createPeerAdminCard.sh
 8. Start the web-app (Playground) : 
     composer-playground
9. Appendix:  Destroy a previous setup 
    docker kill $(docker ps -q)
    docker rm $(docker ps -aq)
    docker rmi $(docker images dev-* -q)