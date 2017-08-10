FROM microsoft/dotnet:latest
RUN sh 'dotnet restore && dotnet publish -c release'
COPY . /app
WORKDIR /app
EXPOSE 5000/tcp
ENTRYPOINT ["dotnet", "run"]
