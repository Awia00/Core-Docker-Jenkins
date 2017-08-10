FROM microsoft/dotnet:latest
COPY . /app
WORKDIR /app
RUN dotnet restore && dotnet publish -c release
EXPOSE 5000
ENTRYPOINT ["dotnet", "run", "--server.urls", "http://0.0.0.0:5000"]
