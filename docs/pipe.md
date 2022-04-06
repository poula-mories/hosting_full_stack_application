# Pipeline


## Jobs of `.circleci/config.yml` pipeline:

### Install job include:

1. get all files from repository
2. install all debendencies `(frontend & backend)`


### Build job include

1. Build typscript files of `(frontend & backend)`

### deploy job include

1. Install AWS CLI 
2. Install & setup Elastic Beanstalk
3. Intialize & use eb environment and set environment variables from CircleCI Context called `udagram_context`
4. Deploy `frontend` to S3 bucket & Deploy `backend` to Elastic Beanstalk