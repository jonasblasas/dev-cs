FROM microsoft/dotnet:2.1-sdk
VOLUME ["/workspace/src"]
WORKDIR /workspace/src/myApp
# restore as distinct layers
RUN dotnet restore

# build everything else
RUN dotnet publish -c Release -o out