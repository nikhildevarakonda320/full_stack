# My Classmates Deployment



*Repo Link*: https://github.com/nikhildevarakonda320/full_stack.git

*Deployment Link*: http://ec2-18-119-126-116.us-east-2.compute.amazonaws.com



## Steps



•⁠  ⁠Choose EC2 and create an instance

•⁠  ⁠choose Amazon Linux

•⁠  ⁠Choose an existing Key Pair or create a new one

•⁠  ⁠Allow All SSH, HTTPS and HTTP requests from anywhere

•⁠  ⁠Create instance

•⁠  ⁠Connect to instance

  *Install git, docker and docker-compose*

•⁠  ⁠⁠ sudo yum update -y ⁠

•⁠  ⁠⁠ sudo yum install -y git docker ⁠

•⁠  ⁠⁠ sudo service docker start ⁠

•⁠  ⁠⁠ sudo chkconfig docker on ⁠ this makes docker AutoStart

•⁠  ⁠⁠ sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose ⁠

  - this downloads docker-compose

•⁠  ⁠⁠ sudo chmod +x /usr/local/bin/docker-compose ⁠ to give permissions to docker-compose

•⁠  ⁠Check if everything's running fine



  - ⁠ git --version ⁠

  - ⁠ docker --version ⁠

  - ⁠ docker-compose --version ⁠



•⁠  ⁠If any private repo is needed to be cloned, we have to setup an SSH key. Follow these [instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=Linux)



•⁠  ⁠Now clone both the repositories

•⁠  ⁠Add the docker-compose.yaml file

•⁠  ⁠Add the contents of the nginx.conf in the ec2's /etc/nginx/nginx.conf file

•⁠  ⁠run ⁠ docker-compose up --build -d ⁠



•⁠  ⁠check at http://ec2-3-89-161-97.compute-1.amazonaws.com



## Usage of AI



•⁠  ⁠I've used ChatGPT to help with writing Dockerfiles and docker-compose files

•⁠  ⁠I configured nginx and made my requests route between frontend and backend using LLMs