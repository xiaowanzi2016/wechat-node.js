var express=require('express');
var router =express.Router();
var wechat=require('wechat');
var config=require('../config.js');
router.use('/',wechat(config,function(req,res,next){
var message=req.weixin;
if(message.FromUserName==='diaosi'){
res.reply('hehe');
}else if(message.FromUserName==='text'){
res.reply({
content:'text object',
type:'text'
});
}else if(message.FromUserName==='hehe'){
res.reply({
type:"music",
content:{
title:"laiduanyinyueba",
description:"yiwusuoyou",
musicUrl:"http://mp3.com/xx.mp3",
hqMusicUrl:"http://mp3.com/xx.mp3",
thumbMediaId:"thisThumbMediaId"
}
});
}else{
res.reply([
{title:'nilaiwojiajiewoba',
 description:'zheshinshenyugaofushuaizhijiandeduihua',
picurl:'http://nodeapi.cloudfoundry.com/qrcode.jpg',
url:'http://nodeapi.cloudfoundry.com/'
}
]);
}
}));
module.exports=router;
