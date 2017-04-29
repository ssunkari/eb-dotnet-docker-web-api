FROM microsoft/dotnet:1.1-sdk-projectjson
COPY . /api
WORKDIR /api
 
RUN ["dotnet", "restore"]
RUN ["dotnet", "build"]
 
ENV ASPNETCORE_URLS http://*:5000
EXPOSE 5000/tcp
 
ENTRYPOINT ["dotnet", "run"]

#https://www.gaui.is/dockerized-web-api-in-net-core/
#http://stackoverflow.com/questions/42159311/deploying-net-core-app-to-docker-gives-microsoft-dotnet-props-not-found-error
#https://hub.docker.com/r/microsoft/dotnet/
#http://blog.scottlogic.com/2016/09/05/hosting-netcore-on-linux-with-docker.html