# Installation and Setup Instructions for Minecraft Server 1.21.11

## Prerequisites:
- Java 17 or newer installed. Verify by running `java -version` in your command prompt or terminal.
- A stable internet connection.
- Sufficient hardware resources: at least 2GB RAM for a small server, 4GB or more for larger servers.

## Step 1: Download the Server Software
1. Go to the official [Minecraft server download page](https://www.minecraft.net/en-us/download/server).
2. Download the Minecraft server .jar file for version 1.21.11.

## Step 2: Create a New Directory
1. Create a new folder where you want to host your Minecraft server.
2. Move the downloaded .jar file into this folder.

## Step 3: Start the Server
1. Open a command prompt or terminal in the directory where your server .jar file is located.
2. Run the command:
   ```bash
   java -Xmx1024M -Xms1024M -jar minecraft_server.1.21.11.jar nogui
   ```
   Adjust `-Xmx` and `-Xms` values based on the available RAM on your machine.
3. This will generate the necessary files and folders for your server, including the `eula.txt` file.

## Step 4: Accept the EULA
1. Open the `eula.txt` file created in your server folder.
2. Change `eula=false` to `eula=true`.
3. Save and close the file.

## Step 5: Configure the Server Settings
1. Open the `server.properties` file to adjust server settings (e.g., server name, game mode, difficulty).
2. Customize settings according to your preference.

## Step 6: Start the Server Again
1. Return to your command prompt or terminal.
2. Run the server command again:
   ```bash
   java -Xmx1024M -Xms1024M -jar minecraft_server.1.21.11.jar nogui
   ```
3. Your Minecraft server should now be up and running!

## Step 7: Connecting to Your Server
- Launch Minecraft on your computer.
- Select “Multiplayer” then click “Add Server”.
- Enter your server address (e.g., `localhost` if you are hosting it locally).

## Troubleshooting
- If the server does not start, ensure that your Java installation is correct and that you are running the command in the directory where the .jar file is located.
- Check your firewall settings to ensure that it permits connections to the server's port (default is 25565).