# redmine
What is Redmine?
Redmine is a free and open source, web-based project management and issue tracking tool. It allows users to manage multiple projects and associated subprojects. It features per project wikis and forums, time tracking, and flexible role based access control. It includes a calendar and Gantt charts to aid visual representation of projects and their deadlines. Redmine integrates with various version control systems and includes a repository browser and diff viewer
here is a manifest file to configure redmine in k8s environment


A. Create two namespace redmine and database
B. Use this docker image to deploy redmine https://hub.docker.com/redmine as
kubernetes deployment in “redmine namespace”
C. Database used should be in “database ” namespace
D. All the credentials wherever required should be passed as kubernetes SECRETS
mounted by volumes
E. All environment variables wherever required should be passed via CONFIGMAPS
mounted a volumes
F. Demonstrate Liveness and Readiness Probe usage
G. Create a network policy in such a way that only allows inbound traffic from “redmine”
namespace to “database” namespace
    
    
Once the redmine is running, mount the config map “”redmine-route” at the location
“/usr/src/redmine/config/routes.rb” .
mount file is given in code itself routes.rb
