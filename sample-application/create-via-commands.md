run redis container

docker run -d  --name=redis redis

run postgree container

docker run -d --name=db postgres:9.4

run python app for voting

docker run -d --name=vote --link=redis:redis -p 5000:80 voting-app

run nodejs for result

docker run -d --name-result -p 5001:80

run dotnet as worker

docker run run -d --link redis:redis --  link db:db --name=worker worker


example: https://github.com/dockersamples/example-voting-app