require('dotenv').config()
var express = require('express')
var app = express()
var bodyParser = require('body-parser')
app.use(bodyParser.urlencoded({ extended: false }))

app.get("/",function(req,res){
    res.sendFile(__dirname+"/form.html")
})

app.post("/form",function(req,res){
    console.log(req.body)
    res.send('Hello')
})
app.listen(process.env.PORT,function(){console.log(`server is running on port ${process.env.PORT}`)})