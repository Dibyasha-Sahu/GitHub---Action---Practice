## Task 1: Key-Value Pairs

Create person.yaml that describes yourself with:

name
role
experience_years
learning (a boolean)

## Task 2: Lists

Add to person.yaml:

tools — a list of 5 DevOps tools you know or are learning
hobbies — a list using the inline format [item1, item2]

## Task 3: Nested Objects

Create server.yaml that describes a server:

server with nested keys: name, ip, port
database with nested keys: host, name, credentials (nested further: user, password)


## Task 4: Validate Your YAML

Install yamllint or use an online validator
Validate both your YAML files
Intentionally break the indentation — what error do you get?
Fix it and validate again

 - I completed task from 1 to 3 ,you can look after the folder .github/workflows
 - To complete the task 4 you have to
   
           - clone the repo to vs code
           - open the terminal and change it to ubuntu for smoother process
           - sudo apt update & sudo apt-get install -y yamllint
           - After this you can check all the indentation and solve all the linters and then run
           - to run your .yml file = yamllint person.yml
