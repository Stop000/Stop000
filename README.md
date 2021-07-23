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

// 當 Bot 接收到訊息時的事件
client.on('message', msg => {
    // 如果訊息的內容是 'ping'
    if (msg.content === 'yagoo, 你的夢想是什麼') {
        // 則 Bot 回應 'Pong'
        msg.reply('我的夢想是要把hololive打造成一個偶像團體');
    }
});

client.login(token);

$ node discord.js
