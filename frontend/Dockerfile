# Installs the current application on a Node Image.
FROM node:10.5
# The qq is for silent output in the console
# You are welcome to modify this part as it
# Sets the path where the app is going to be installed
ADD . /frontend
WORKDIR /frontend
COPY . /frontend
# Install all the packages
RUN npm install -g @angular/cli
RUN yarn install


CMD ng serve --host 0.0.0.0 
EXPOSE 4200 
