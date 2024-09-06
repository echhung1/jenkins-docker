# Jenkins build

simple docker compose script to spin up a jenkins instance with java and maven built into the image. This
is so that you can build a pipeline job very quickly and shows the basics of a working pipeline .

## How to get setup
1. make sure you have docker running and installed on your machine 
2. clone repo
3. change the volume from /SOMEWHERE/ON/YOUR/MACHINE
4. run "chmod +x jenkinsUp.sh" 
5. run ./jenkinsUp.sh
6. go to localhost:8080 on your browser
7. Follow the jenkins prompts
8. install the recommended plugins and change the inital password - the initial admin password for jenkins should be logged out in your terminal where you ran ./jenkinsUp.sh
9. login to jenkins
10. create a jenkins pipeline job by clicking on new item on the top left and selecting pipeline
11. copy the script from Jenkinsfile into the pipeline script box at the bottom of the page
12. click build now
13. congratulations you should have a working jenkins pipeline job

## How to shutdown the jenkins container
1. run 'docker compose down'

## How to bring the instance back up
1. run ./jenkinsUp.sh  (you can also run "docker compose up")





## TODO
- [ ] configure a jenkins agent with master jenkins
