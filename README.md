# Dapr Actor Model With Net 6

In this example I show you a small example of using actors with Dapr and .NET6

# Steps

1. Run dapr unistall and use the latest version, I used 1.7.4
   ```
   dapr unistall
   ```
2. Install Dapr and now you can access to dashboard & you must show redis & Zepkin
   ```
   dapr install
   ```
3. Go to the folder DaprActorSample.ActorsHost and run:
   ```
   dapr run --app-id actorhost --app-port 3000 --dapr-http-port 3500 -- dotnet run
   ```
4. Go to the folder DaprActorSample.Test and run:
   ```
   dapr run --app-id actorclient --dapr-http-port 3600 -- dotnet run
   ```
Now you can view the use of the actors in the output.