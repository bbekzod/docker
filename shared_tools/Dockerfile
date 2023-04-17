FROM  ubuntu:16.04
RUN  apt  update 
RUN  apt install  -y  wget  unzip 
# install terraform 
RUN wget https://releases.hashicorp.com/terraform/1.4.5/terraform_1.4.5_linux_amd64.zip
RUN unzip terraform_1.4.5_linux_amd64.zip   
RUN chmod  +x terraform  
RUN mv  terraform  /usr/local/bin/
    
# # install packer
RUN wget https://releases.hashicorp.com/packer/1.8.6/packer_1.8.6_linux_amd64.zip
RUN unzip packer_1.8.6_linux_amd64.zip
RUN chmod  +x packer
RUN mv  packer  /usr/local/bin/
# install gcloud
RUN apt-get update && apt-get install -y curl apt-transport-https ca-certificates gnupg
RUN echo "deb [signed-by=/usr/share/keyrings/cloud.google.gpg] https://packages.cloud.google.com/apt cloud-sdk main" |  tee -a /etc/apt/sources.list.d/google-cloud-sdk.list
RUN curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key --keyring /usr/share/keyrings/cloud.google.gpg add -
RUN apt-get update &&  apt-get install google-cloud-sdk
# install aws cli
RUN apt-get install -y curl 
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip 
RUN ./aws/install

