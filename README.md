# module.exports

module.exports = {
    name: "",
    usage: ["``"],
    description: '',
    example: ["``"],
    enabled: true,
    aliases: [""],
    category: "",
    memberPermissions: [ "" ],
    botPermissions: [ "", "" ],
    nsfw: false,
    ownerOnly: false,
    cooldown: 5000,
    
    //Wykonanie komendy
    async execute(client, message, args, data){
        try{



        }catch(err){
            client.logger.error(`Wystąpił błąd w komendzie: ${data.cmd.name}`)
            console.log(err)
            return client.embed.send(message, {
                description: `Wystąpił nieoczekiwany błąd, jeżeli bedzie się dalej powtarzał - zgłoś się do naszego dev. teamu!.`,
                color: `RED`,
                title: ':outbox_tray: Krytyczny błąd komendy'
            });
        }
    }
}"# vavebot" 
