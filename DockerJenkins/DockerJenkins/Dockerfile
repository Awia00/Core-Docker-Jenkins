FROM microsoft/dotnet:latest
RUN dotnet restore && dotnet publish -c release
COPY . /app
WORKDIR /app
EXPOSE 5000
ENTRYPOINT ["dotnet", "run"]
