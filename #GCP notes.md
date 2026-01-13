#GCP notes
# what is Linux
- Linux is and open source Operating system
-Other operating systems includes MacOS ,Microsoft operating system
# package manager in Linux
- Red Hat ; Yum or dnf
-Ubuntu : apt
# Distribution center in Linux
- red Hat (RHEL): centOs and fedora
_Ubuntu :Debian (Free)

# Linux Server
- Linux  can be use as a server and and as an OS,
Most Databases , Web servers and email Servers run on Linux Server .

# using Linux as a desktop
- You can use  Linux daily with a limit .
Ubuntu Desktop  is very light 
# why we use Linux  over windows
-Low cost
-Efficeint

# Using Linux
SSH(secure Shell)
- To SSH to a server you need  transport , Authentication and connection .
the Protocol allows a sercured connection
_ Scp to transfer file 
- Ssh used keypaired connection for sercurity
-Both Linux and windows can you use other programs other than SSH to connect
-Windows uses a Free program called putty

# Update and Install software in Linux
 its not good to update your software as a root user
 -its good you use the Sudo cmd
 # CLI or GUI 
 the CLI is available for all Linux distrubution

# Sercurity in Linux
- give acess to only those who need it
-keep data safer but available
- Use firewalls and acess control
-close ports for outside traffic when not in use
- internal firewalls can be used for purporse

     # GIT
-Git helps us to work as a team , see changes in the file
-In git a repository is a collection of various different projects
- we can install git on our machine depends on the OS  ( for ubunto we use git ap install git , for redhat we use yum install git) and we need to be the sudo user 
-git branche (creats  a NEW branch)
-git checkout branchname (switch to the branch)
-git checkout -b branchname (creats and switch to the branch)
-git log (helps us to know more details about what was being modified , who , time and more details)
-Main or masters are the default branches .

  # BASH SCRIPT 
  - bash scripting is the use of command to automate processes
  - Bash S always starts with a Shebang  that is #!/bin/bash
  - grep : use for search
  - sort : input and prints a sorted output
  ** VARIABLES***
  - Variables 

    *************** # INTRODUCTION TO GOOGLE CLOUD
    -GC offers platform as a service , and infrastructure as a service
    it also prove cloud services such as data storage , machine learning ,data anylytics(big data) ,networking and computing
    - Cloud computing : its the use of hardware and software components to deliver a service to a network. Users can cess these files and apllication for any device that can access the internet
     # Break down of google cloud services
     1) COMPUTE : the compute sercices allows for compute and hosting the cloud this includes
     . app engine
     .compute engine
     .kubernetes Engine
     .cloud fonctions
     .cloud run
     2) STORAGE AND  DATABASE
     .Cloud storage
     .cloud SQL
     .cloud big table
     .cloud spanner
     .persitent disc
     .cloud memoryStore

     3) NETWORKING

     .VPC
     .Cloud Load balancer
     . cloud CDN
     .Cloud DNS
     .cloud Armor
     .Cloud interconnect
     .Network service Tiers

     4) Developer tools

     .Cloud SDK
     .development manager
     .cloud source repository
     .cloud test lab
     5) BIG DATA
     6) IDENTITY AND SERCURTY 
     .cloud identity
     .cloud IAM - when you talk about Cloud I AM 
     .Cloud Key management
     7) Cloud AI
     8) Cloud API



    # what makes  Google Cloud diffrenet from the others
    - Google sercurity model (first-rate sercurity )
    - pribate fiber Global network ( Global presence of Data center)
    - dedicated to machine learning and big data
    - live Migration
    - Afordable Price
    - Speed (low letency network infrastructure) and availabilty (minimal downtime)
    - customer support 
    - easy to use cloud services

    # GCP Cloud - Regions and Zones
    we are  Multiple Region
            |
          Region
            |
            
          Zone
 

    # Google Cloud Api
    -Google cloud Apis all you to access Google  product from the consol or code
    # IAM in GCP
    - it also  to give someone permission for a  role ,
     - sercurity

     # organization
     - when we talk of organization  we talk about the  hierachy of google cloud resources which is as fellow : Organization (root node of the hierachy)>Folder> Projects
     # what are Google Cloud Projects ?
- A project consist of a set of users , set of API and bills , authentification and monitoring setting for those ApIs 
     # Understanding Network design in Google cloud
_ A VPC is a virtual version of a physical network , implemented isnide of the Googles Production network .

   # Compute  Engine
   # Cloud storage 
-  Cloud Storage provide a storage class for any worklaod.
-Storage clasee
a) Standard : its best for data that are requently access for a brief period of time(short term) .
b) Nearline Storage Class : its a low cost storing infrequent access data
c) Coldline Storgae Class: its similar to nealine SC  but the Coldline is best bc you can acess once in a quaterG .
d) Archive SC: its a the lowest cost highly durable for achieving data backup and disaster receovery(can be acess once a year)

  # what time of Data Base does GCP  offer

  a database is an organise collection of data stored in a compute system ; we have  relational DB ( has structured data are usually in column and rows eg Cloud SQL , cloud spanner) and non relational DB (eg big Table , firestore and memory store)

  # Analytics 
  - collect store , process and analyze large amount of data 

  # Big Query
- big query is a serverless , highly scalable  and cost effective multi data warehouse designed for business agility .
- Big query is a data warehouse that allows massive processing of data at high speed.
- Big query have some capabity to run some machine learning Algarithms 

# Google Dataflow
 its a fully managed service for executing apache beam pipeline with the google Cloud platform  ecosystem . its helps to build our pipeline from scratch and its a cloud native tool.
 - Dataflow can helps us move data from on prem to cloud 

# Composer ;
- its helps to orchestrate our ETL job

# Pub/Sec 
 its a messaging service 

# DATA Proc 
- Helps to manage the transfer of Big data from onprem to Cloud 

# GCP sercurity
-by encrption in transit and encryption at rest of data.
-sercure internet connection
- IAM

# how resources are Monitoring in GCP
- we do this by creating a monitoring dashboard

# Machine leaning and AI
- Machine learning : the goal of machine learning is to build a computer systems that can adapt and learn from their experience thats is to laern from me or the customer .
Artificial  intelligent goal is to build a computer system that can learn from you and also predict behavior and asnwer question you

# CICD
- the CICD tool for GCP is cloud build . it helps to build , test and deploy application using a severless CICD platform


aws s3api put-object --bucket ai-pipeline-access-allowed-bucketcad0 --key input/raw-audio/

aws s3api put-object --bucket ai-pipeline-access-allowed-bucketcad0 --key input/raw-text/

aws s3api put-object --bucket ai-pipeline-access-allowed-bucketcad0 --key output/transcripts/

aws s3api put-object --bucket Yai-pipeline-access-allowed-bucketcad0 --key output/nlp-insights/



aws s3api put-object --bucket ai-pipeline-access-denied-bucketcad0 --key input/raw-audio/

aws s3api put-object --bucket ai-pipeline-access-denied-bucketcad0 --key input/raw-text/

aws s3api put-object --bucket ai-pipeline-access-denied-bucketcad0 --key output/transcripts/

aws s3api put-object --bucket ai-pipeline-access-denied-bucketcad0 --key output/nlp-insights/