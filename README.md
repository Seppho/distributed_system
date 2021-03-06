# A Distributed System using hadoop
This is the project for the course "Distributed Systems 1"

## First Steps
1. Install java, python, node and git and config local path.

    <code>sudo apt-get install openjdk-8-jre openjdk-8-jdk vim git</code>

    <code>echo "export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64/jre/" >> ~/.bashrc</code>

    <code>echo "export HADOOP_HOME=~/hadoop" >> ~/.bashrc</code>

2. Download hadoop 2.8 and unzip it in your home folder

    <code>wget http://it.apache.contactlab.it/hadoop/common/hadoop-2.8.0/hadoop-2.8.0.tar.gz</code>

    <code>tar xvf hadoop-2.8.0.tar.gz</code>

    <code>mv hadoop-2.8.0 ./hadoop</code>

3. configure hadoop to run as pseudo distributed system

    <code>source ~/.bashrc</code>

4. generate and add ssh key into authorized_keys

    <code>
        ssh-keygen -t rsa -P '' -f ~/.ssh/id_rsa
        
        cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
        
        chmod 0600 ~/.ssh/authorized_keys
    </code>

4. clone the repository and run ./start.sh

    <code>git clone https://github.com/seppho/distributed_system</code>
    
    <code>
        cd distributed_system
        
        ./start.sh
    </code>



## Useful links
NameNode at http://localhost:50070

ResourceManager at http://localhost:8088

MapReduce JobHistoryServer at http://localhost:19888
