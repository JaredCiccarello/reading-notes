May 19, 2023

~9:05~ Warm up
require ('doenv').config():

const express = require (express);
const cors = require('cors');
const app = express ()
app.use(cors())

const PORT = process.env.PORT || 3002;

app.get('username', (request, response) => {
    userInfo.name = request.username;
    userInfo.password = request.password;

    response.send(userInfo);
})
app.listen(PORT, ())




~9:25~ Code challenge 09 Review

Question Code challenge 

What goes into a callaback? A name we declare. 








It's not unusual 

