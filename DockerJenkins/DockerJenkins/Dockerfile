# FROM microsoft/dotnet:latest
FROM microsoft/dotnet:2-runtime-stretch-arm32v7
COPY . /app
COPY out ./
WORKDIR /app
RUN dotnet restore 
RUN dotnet publish -c release
EXPOSE 5000
ENTRYPOINT ["dotnet", "run"]
