# Dockerfile for your published ASP.NET Core app
FROM mcr.microsoft.com/dotnet/aspnet:8.0 AS base
WORKDIR /app

# Copy all files from current folder into container
COPY . .

# Configure Kestrel to listen on the PORT Render/hosts will provide
ENV ASPNETCORE_URLS=http://+:8080
ENV PORT=8080

# Start the app (use your DLL name)
ENTRYPOINT ["dotnet", "WebApplication1.dll"]
