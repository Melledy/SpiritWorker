# SpiritWorker
A WIP server emulator for SoulWorker (GF 1.7.20.2). Currently, you can spawn in the world, give yourself items, and play the very first dungeon.

# Running the server and client

### Prerequisites
* Java 8 JDK
* Mongodb (recommended 4.0+)
* GF soulworker client (1.7.20.2 or 1.7.21.2) installed

### Starting up the server
1. Compile the server with `./gradlew jar`
2. Extract the .res files from data12.v in your soulworker client/data folder into a folder called resources in your spiritworker directory (use something like https://github.com/Leayal/VData-Reader)
3. Copy the `data` folder from the source folder to your server directory
4. Run the server with `java -jar spiritworker.jar`, you can also run both the auth and game servers separately by adding -auth or -game as an argument

### Connecting with the client
Run the client with `SoulWorker.exe --authCode aaaaa --ip 127.0.0.1 --port 9000` as its launch arguments

### In game commands
`!give [item id] [count]` - Gives {count} amount of {item id}

`!starterpack` - Gives you a full set of the Vistor's armor and Tathata’s jewelry

`!changestat [stat id] [value]` - Sets one of your stats to {value}
