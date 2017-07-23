# AgentK
A chatbot to solve support issues

## Execution instructions
Makes sure ChatterBot py, link: https://chatterbot.readthedocs.io/en/stable/setup.html , is installed

### Running MongoDB:
Installation Instructions: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/

1. curl -O https://fastdl.mongodb.org/osx/mongodb-osx-x86_64-3.4.6.tgz

2. tar -zxvf mongodb-osx-x86_64-3.4.6.tgz

3. mkdir -p mongodb

4. cp -R -n mongodb-osx-x86_64-3.4.6/ mongodb

5. export PATH=<mongodb-install-directory>/bin:$PATH

6. mkdir -p /mongdb/data/db

7. mongod --dbpath <path to data directory>

### Execute the file:
python agentK.py

This trains using the default English corpus available and sets up a mongodb to store the data.

## TODO:
1. Add naive bayes classification to classify incoming questions

2. Add a mariadb sql adapter to work with mariadb mysql databases (just for investigation)

3. Add a logic adapter that can verify if a website is up and running or not

4. Able to respond to questions of the form: "Tell me more about X", "What is X", "What to do about X" 