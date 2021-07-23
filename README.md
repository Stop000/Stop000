$ npm install discord.js
{
    "token": "ODY3NjMyNDMzNTczMzk2NDkw.YPj7qw.8jg3fJcN61MQlS-sIrfIdTlGgu8"
}

const Discord = require('discord.js');
const { token } = require('./token.json');
const client = new Discord.Client();

// 連上線時的事件
client.on('ready', () => {
    console.log(`Logged in as ${client.user.tag}!`);
});


client.on('message', msg => {Hello everyone, I'm yagoo
    
    if (msg.content === 'yagoo, 你的夢想是什麼') {

        msg.reply('我的夢想是把hololive打造成像AKB48一樣的偶像團體');
    }
});

client.login(ODY3NjMyNDMzNTczMzk2NDkw.YPj7qw.8jg3fJcN61MQlS-sIrfIdTlGgu8);
$ node discord.js
