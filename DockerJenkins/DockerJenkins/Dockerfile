FROM microsoft/dotnet:latest
COPY . /app
WORKDIR /app
EXPOSE 5000
RUN dotnet restore && dotnet publish -c release
ENTRYPOINT ["dotnet", "run"]
