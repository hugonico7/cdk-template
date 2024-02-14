FROM --platform=linux/amd64 node:18-slim

# Install aws-cdk and TypeScript globally. Update de system and install awscli
RUN apt update\
 && apt install -y git curl unzip\
 && npm install -g aws-cdk typescript\
 && curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"\ 
 && unzip awscliv2.zip\ 
 && ./aws/install

CMD [ "sleep", "infinity" ]