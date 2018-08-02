# socketChatSystem

Koma þessum kóða inní þannig að virki inní routes/index.js

var http = require('http').Server(app);
const io = require('socket.io')(http);

io.on('connection', function(socket){
    socket.on('chat message', function(msg){
        io.emit('chat message', msg);
    });
});;
