# SCA-Cloud-School-Application

### Setting up your workspace

Before running this app locally make sure you have the following software installed:

-   node.js
-   NPM
-   Docker

### steps to solving task:

1. I created a repository and initialized my project file on github
2. I cloned the project to my PC `git clone url`
3. Then I checked out to a new branch called start `git checkout -b start`
4. I created an `app.js` file where my script was written
5. I ran `npm init -y` and `npm install express` to add my `package.json `  and `package-lock.json`file
6. I ran `node app` to make sure my script was running on `http://localhost:8080`
7. I created a `Dockerfile` in the root directory which packages my node.js file in a container
8. I created a `.dockerignore` file and added the node modules
9. I created a docker hub account
10. Then I built the image from the Dockerfile by running `Docker build -t eel30/sca-node-app .`
11. I ran the container with `Docker run -p 8080:8080 -d eel30/sca-node-app`
12. I ran my script on the browser using `http://localhost:8080`
13. I commited the my files and pushed the start branch to github with `git push origin start`
14. I updated my script message as required 
15. Then I repeated the build process again with `Docker build -t eel30/sca-node-app .`
16. I also ran the container again with a different port `Docker run -p 8081:8080 -d eel30/sca-node-app`
17. Then I ran my script on the browser using `http://localhost:8081`
18. Then I checked out to a new branch called feature `git checkout -b feature`
19. I commited the updated script into the feature branch
20. Then I merged the feature branch to the start branch
21. I pushed the feature branch to github with `git push origin feature`
22. I ran `docker ps -a` to check if my container was running
23. Then I ran `docker login` to log into my docker account
24. Then I pushed my project to my docker hub repository with `docker push eel30/sca-node-app:latest`
25. I then checked out to main branch with `git checkout main`
26. I updated the readme file
27. Then push to the main branch on github

NB: I didn't store the docker related files in a docker folder because the docker file should be in the root of my application folder so I can view the image and run the container.


Link to dockerhub repo [https://hub.docker.com/repository/docker/eel30/sca-node-app](https://hub.docker.com/repository/docker/eel30/sca-node-app)