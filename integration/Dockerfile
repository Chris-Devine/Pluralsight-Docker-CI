FROM microsoft/dotnet:2-sdk

WORKDIR /integration

# restore
COPY integration.csproj .
RUN dotnet restore

COPY . .
ENTRYPOINT ["dotnet", "test"]
