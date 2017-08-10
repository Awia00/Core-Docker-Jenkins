FROM microsoft/dotnet:latest
COPY . /app
WORKDIR /app
EXPOSE 5000/tcp
RUN dotnet restore && dotnet publish -c release
ENTRYPOINT ["dotnet", "run"]
