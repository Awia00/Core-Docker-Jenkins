FROM microsoft/dotnet:latest
COPY . /app
WORKDIR /app
RUN dotnet new mvc && dotnet restore && dotnet publish -c release
EXPOSE 5000
ENTRYPOINT ["dotnet", "run"]
