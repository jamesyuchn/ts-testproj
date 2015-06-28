# ts-testproj
Two servers from socket.io, added redis to make them connectable to each other.

1. Install redis at localhost:6379, which is default installation. Start redis.

2. Clone this project to any place. 

3. Open two terminals and cd into 'socket.io-master/example/chat' and  'socket.io-master-cp/example/chat'

4. Run `node index.js` seperately in both terminals

5. Open browser and go to localhost:3000 and localhost:3001, they can communicate with each other

6. If comment line 'io.adapter(redis({ host: 'localhost', port: 6379 }));' in both index.js file and rerun, they cannot see each other
