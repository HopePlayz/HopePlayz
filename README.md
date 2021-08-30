const Discord = require ("discord.js")
const client = new Discord.Client()
client.once("ready",() =>{
 console.log('${client.user.tag} is now 
         online!')
});
client.on("message",async message =>{ 
if (message.content.startsWith("!ping"))
{
   message.channel.send('The client 
    websocket latency is ${client.ws.ping}ms (values in milliseconds)')
  } 
})
client.on("guildMemberAdd"; async member
=> , { 
let channel = member.guild.channels
  .cache.find(c => c.name === 'welcome')
let Welcome = new Discord.MessageEmbed()
.setTitle('New user has Joined!') 
. setDescription('Welcome to Our Server
${member.tag} we are happy to have you! You are member number ${member.guild.memberCount}!')
.setColor('YELLOW')
.setTimestamp()
.setFooter('Thanks for Joining!')
channel.send(WELCOME

})
client.login("BOTTOKENHERE");
