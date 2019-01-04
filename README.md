This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

I used this tutorial to set up this example of running react with docker

[https://mherman.org/blog/dockerizing-a-react-app/](https://mherman.org/blog/dockerizing-a-react-app/)

[https://medium.com/@tiangolo/react-in-docker-with-nginx-built-with-multi-stage-docker-builds-including-testing-8cc49d6ec305<Paste>](https://medium.com/@tiangolo/react-in-docker-with-nginx-built-with-multi-stage-docker-builds-including-testing-8cc49d6ec305)

### Comands

* Build and tag the Docker image: `docker build -t sample-app .`;
* Build compose the image and fire up the container: `docker-compose up -d --build`;
* Run: `docker run -it \
  -v ${PWD}:/usr/src/app \
  -v /usr/src/app/node_modules \
  -p 3000:3000 \
  --rm \
  sample-app`;
* Run composer: `docker-compose up sample-app`


## Comands prod

* `docker build -f Dockerfile-dev -t hamaka-dev .` Build and tag the docker image;
* `docker-compose -f docker-compose-dev.yml up -d --build` - Build compose the image and fire up container
* `docker-compose -f docker-compose-dev.yml up` Up application:;
