ssh-keygen -t rsa -m PEM -f remote_key

docker-compose build

docker-compose up -d

sudo apt-get install openssh-client