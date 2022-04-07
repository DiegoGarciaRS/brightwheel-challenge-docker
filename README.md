# brightwheel-challenge-docker

 * Clone this repo locally
 * Navigate on terminal to the location
 * On AWS Console --> Create ECR repository
 * Follow indicated Steps, they will be similar to the ones below:

aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 458572724268.dkr.ecr.us-east-1.amazonaws.com

docker build -t brightwheel-challenge .

docker tag brightwheel-challenge:latest 458572724268.dkr.ecr.us-east-1.amazonaws.com/brightwheel-challenge:latest

docker push 458572724268.dkr.ecr.us-east-1.amazonaws.com/brightwheel-challenge:latest
 * Go to the terraform repository and follow steps there
 https://github.com/DiegoGarciaRS/brightwheel-challenge