# Coding Kata Workshop

Kata is a Japanese word, meaning a detailed choreographed pattern of movements made to be practiced alone or within groups when training.

> Kata is a also term used by software engineers in the Software Craftsmanship movement. 
> Software Engineers who call themselves Software Craftsmen, will write Kata.
> Software Kata is a small snippet of code written in one sitting, repeatedly, often daily, in order to build up muscle memory and practice their craft.

This workshop aims to provide you with some kata exercises that you can practice. We will go over some of the techniques to focus and pratice your kata, and solve problems differently. These exercises vary from general to more complex algorithms. Remember that coding katas are for practice and improving your skills. You should try to solve it and also find a good solution following best practices of software development. Code Kata is a way to bring these element of practice to software development.

Key points to keep in mind:

1) Repeat a task many times and make litte improvement in each time.
2) Build up muscle memory on specifc tasks. Remember stuff you learned along the way.
3) Short exercise (30 - 45 min long)
4) Programming to solve similar problems in different ways. 
5) The goal of coding kata is not getting to the final solutions. The goal is to practice regulary. 


A good coding kata practice sesison would be as follows:

1) A time without interruptions
2) A simple thing you want to try as many times as it takes
3) Review any mistakes that you made and learn from it
4) Look for feedback each time and work to improve
5) No pressure and no deadline


# The Bowling Game Kata

The bowling game consists of 10 frames.  
In each frame the player has two opportunities to knock down 10 pins.  
The score for the frame is the total number of pins knocked down, plus bonuses for strikes and spares.

A spare is when the player knocks down all 10 pins in two tries.  
The bonus for that frame is the number of pins knocked down by the next roll.  

A strike is when the player knocks down all 10 pins on his first try.  The bonus
for that frame is the value of the next two balls rolled.

In the tenth frame a player who rolls a spare or strike is allowed to roll the extra
balls to complete the frame.  However no more than three balls can be rolled in
tenth frame.


# Git Kata

You will be working in your own branch. This time we will be working with branches in git.

1) Create a branch called greeting and check it out
2) Edit the greeting.txt to contain your favorite greeting
3) Add greeting.txt files to the staging area
4) Commit
5) Switch back to the master branch
6) Create a file README.md with information about this repository
7) Add the README.md file to staging area and make the commit
8) What is the output of git log --oneline --graph --all?
9) Diff the branches
10) Merge the greeting branch into master


# Linux Kata

1) Create two users, Ravi and Kumar
2) Make them members of the second group SystemAdministrators
3) Ravi should have interactive login shell
4 )Kumar should have no login shell
5) Create an collaborative directory path /dir/data
6) The directory should be owned by SystemAdministrators
7) All files created under this directory should have group permissions
8) Others should not have any access to this directory#


# Openshift Nexus Kata

1) Create a new project named username-nexus with display name Shared Nexus.
2) Deploy the Nexus container image and create a route to the Nexus service. 
3) Pause the automatic deployment upon configuration changes.
4) Change the deployment strategy from Rolling to Recreate and set requests and limits for memory.
5) Create a persistent volume claim and mount it at /nexus-data.
6) Set up liveness and readiness probes for Nexus.
7) Resume deployment of the Nexus deployment configuration to roll out all changes at once.


# Openshift SonarQube Kata

1) Create a new project called username-sonarqube with a display name of Shared Sonarqube
2) Deploy a persistent PostgreSQL database.
3) Pick values for the POSTGRESQL_USER, POSTGRESQL_PASSWORD, POSTGRESQL_DATABASE, and VOLUME_CAPACITY parameters.
4) Make sure that your database is fully up before moving to the next step.
5) Deploy the SonarQube image (wkulhanek/sonarqube:6.7.5) available in DockerHub.
6) The image expects SONARQUBE_JDBC_USERNAME, SONARQUBE_JDBC_PASSWORD, and SONARQUBE_JDBC_URL in the environment.
7) The correct setting for SONARQUBE_JDBC_URL is SONARQUBE_JDBC_URL=jdbc:postgresql://postgresql/<dbname> where "<dbname>" is the name you picked when you set up PostgreSQL.
8) The source for the Docker image is located at https://github.com/wkulhanek/docker-openshift-sonarqube.git.
9) Pause rollouts for the created SonarQube deployment configuration.
10) Set the following parameters

Memory request: 1.5Gi
Memory limit: 3Gi
CPU request: 1 CPU
CPU limit: 2 CPUs
Set the deployment strategy.

Because SonarQube is using Elasticsearch under the covers, it needs a Recreate deployment strategy rather than the default Rolling deployment strategy.

11) Add liveness and readiness probes.
12) Resume deployment of the SonarQube deployment configuration to roll out all changes at once.
13) After SonarQube has fully started, log in via the exposed route. The default user ID is admin and password is admin.
