# Jenkins build

simple docker compose script to spin up a jenkins instance with java and maven built into the image. This
is so that you can build a pipeline job very quickly and shows the basics of a working pipeline .

## How to get setup
1. clone repo
2. change the volume from /SOMEWHERE/ON/YOUR/MACHINE
3. run "chmod +x jenkinsUp.sh" 
4. run ./jenkinsUp.sh
5. Follow the jenkins prompts
6. create a jenkins pipeline job and configure
7. copy the script in from Jenkinsfile into the script
8. click build now
9. congratulations you should have a working jenkins pipeline job

## How to shutdown the jenkins container
1. run 'docker compose down'


## TODO
- [ ] configure a jenkins agent with master jenkins
