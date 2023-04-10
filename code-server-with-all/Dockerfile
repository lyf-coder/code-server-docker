FROM linuxserver/code-server:latest

# install 16.x nodejs
RUN curl -sL https://deb.nodesource.com/setup_16.x | sudo bash
RUN sudo apt-get install -y nodejs

# install make tool 
RUN sudo apt-get install make

# install pnpm
RUN sudo npm install -g pnpm

# install git cz tool
RUN  sudo npm install commitizen cz-conventional-changelog -g && echo '{ "path": "cz-conventional-changelog" }' > ~/.czrc

# install golang
RUN sudo apt-get install golang --fix-missing
