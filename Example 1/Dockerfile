# https://docs.docker.com/get-started/02_our_app/
FROM node:18-alpine

WORKDIR /app

COPY . .

RUN yarn install --production

RUN mkdir test 

RUN cd test 

RUN touch newfile

CMD ["node", "src/index.js"]


#EXPOSE 3000


# RUN yarn install: Installs the dependencies listed in package.json.
# Yarn reads package.json and the yarn.lock file to install the specified versions of each dependency, 
# which helps ensure consistent builds.
# --production: Installs only the production dependencies (those listed outside the devDependencies section of package.json). 
# This option excludes packages that are only needed for development or testing, 
# which can reduce the size of the final Docker image and improve performance.
