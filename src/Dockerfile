FROM mcr.microsoft.com/dotnet/sdk:8.0-windowsservercore-ltsc2022
COPY . ./app
WORKDIR /app
RUN dotnet workload install maui-windows
RUN dotnet build -c Release
EXPOSE 80
CMD ["dotnet", "run"]