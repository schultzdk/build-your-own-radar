## How to use

Make changes in code and data

    $ npm run build

Commit and push to origin/master

The azure site on https://schultz-teknologivision.azurewebsites.net/ will automatically fetch the new build from github

### Deploy as container in Azure

https://docs.microsoft.com/en-us/azure/container-instances/container-instances-tutorial-prepare-app

### Don't want to install node? Run with one line docker

     $ docker run -p 8080:8080 -v $PWD:/app -w /app -it node:7.3.0 /bin/sh -c 'npm install && npm rebuild node-sass && npm run dev'

After building it will start on localhost:8080