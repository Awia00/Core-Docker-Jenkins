# FROM microsoft/dotnet:latest
FROM microsoft/dotnet:2-runtime-stretch-arm32v7
COPY . /app
WORKDIR /app
RUN dotnet restore && dotnet publish -c release
EXPOSE 5000
ENTRYPOINT ["dotnet", "run"]
