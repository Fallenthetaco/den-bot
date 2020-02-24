# Image Hosting Website for the Alcremie-B Discord Bot ![Bot PFP](https://raphgg.github.io/den-bot/data/icons/botpfp.png "Lovely Baby")
A Pokèmon statistics Discord bot with the intended purpose of facilitating Max Raid Battles in Pokèmon Sword & Pokèmon Shield.

## Discord Usage
[Invite](https://discordapp.com/api/oauth2/authorize?client_id=663505910580248587&permissions=0&scope=bot "Alcremie-B w/ No Permissions") Alcremie-B to your own Discord Server!

## Features 
* Quick and fully featured access to latest Pokèmon Data, such as: Base Stats / Abilities / Den Locations / And more!
* Fully implemented catch rate calculator for Pokèmon encountered in raids.
* Fast Den Information look-up including Pokémon lists and Hidden Ability availability.
* Configurable settings to allow Server Admins to automate role pinging.

## Commands
* `[ ]` Indicate Required Fields
* `( )` Indicate Optional Fields
* Use * on Pokèmon Fields for shiny sprites

| Command       | Arguments                | Descrition                                                                 |
|---------------|--------------------------|----------------------------------------------------------------------------|
| `%catch`      | `[Pokèmon] (Form) (Ball)`| Shows a detailed summary of catch rates for a given Pokèmon & Ball         |
| `%den`        | `[Den #] / [Pokèmon]`    | Shows a list of Pokèmon that belong to a den including their HAs           |
| `%pokedex`    | `[Pokèmon]`              | Shows a detailed summary of a Pokèmon's latest Statistics (Gen 8 / Gen 7)  |
| `%ball`       | `[Ball]`                 | Shows a summary of a Poké-Ball's statistics                                |
| `%natures`    |                          | Displays an in-depth Pokémon natures chart from Bulbapedia                 |
| `%ping`       | `[Role]`                 | Pings the specified role without setting it to be pingable by everyone     |
| `%showconf`   |                          | Displays the server's current bot settings in a JSON Format                |
| `%setconf`    | `[Setting] [Value(s)]`   | Sets the specified setting's value(s)                                      |
| `%resetconf`  |                          | Resets the server's current bot settings to default                        |
| `%help`       |                          | Displays a help message with this table of commands                        |
| `%latency`    |                          | Pings the bot's & discord's API and returns the latency in milliseconds    |
| `%credits`    |                          | Displays a credit and thanks message                                       |

## Configuration Settings
The bot has a selection of configuration settings that can be changed by the server owner or a registered server admin. The full list of settings along with examples on how to use them are listed below:

  `%setconf prefix (Non-alphanumeric Character)`
  Sets the bot's prefix for your server to a given character: `%setconf prefix !`

  `setconf denpkmnonly (true | false)`
  Toggles between fetching Pokèmon statistics from only those that can appear in Sword and Shield Max Raid Dens: `%setconf denpkmnonly true`

  `%setconf shinypkmnonly (true | false)`
  Toggles between displaying shiny Pokèmon sprites only: `%setconf shinypkmnonly true`

  `%setconf restrictedchannels (channel-one, channel-two, etc)`
  Restricts Alcremie-B to only respond in the channels listed. Alcremie-B will respond to server admins and server owner regardless of this setting: `%setconf restrictedchannels alcremie-test, botspam`

  `%setconf adminroles (Admin Role 1, Admin Role 2, Etc.)`
  Allows specified roles to access Alcremie-B's admin only commands (setconf, showconf, resetconf, ping): `%setconf adminroles Admin Role 1, Admin Role 2`

  `%setconf pingroles (Ping Role 1, Ping Role 2, Etc.)` (Obsolete following newest Discord Update)
  Allows specified roles to be pinged by the `%ping` command: `%setconf pingroles Ping Role 1`

The following is what `%showconf` would look like after performing each of the above example commands:

```json

{
 "prefix": "!",
 "denpkmnonly": true,
 "shinypkmnonly": true,
 "restrictedchannels": [
  {
   "name": "alcremie-test",
   "id": "ID#"
  },
  {
   "name": "botspam",
   "id": "ID#"
  }
 ],
 "roles": {
  "adminroles": [
   {
    "name": "Admin Role 1",
    "id": "ID#"
   },
   {
    "name": "Admin Role 2",
    "id": "ID#"
   }
  ],
  "pingroles": [
    {
      "name": "Ping Role 1",
      "id": "ID#"
    }
  ]
 }
}

```

## Example Images
`%catch gmax gengar`

![Catch Gengar Gmax](https://raphgg.github.io/den-bot/data/readme/catchgengargmax.png "Big Baby Boy")

`%catch gmax gengar fast`

![Catch Gengar Gmax Fast](https://raphgg.github.io/den-bot/data/readme/catchgengarfast.png "Speedy Boy 😳")

`%catch gmax gengar timer`

![Catch Gengar Gmax Timer](https://raphgg.github.io/den-bot/data/readme/catchgengartimer.png "He eats the clocks")

`%catch gmax appletun`

![Catch Appletun Gmax](https://raphgg.github.io/den-bot/data/readme/catchappletungmax.png "Promoted Apple of my Eye")

`%den 23`

![Den 23](https://raphgg.github.io/den-bot/data/readme/den23.png "Den Info!")

`%den frosmoth`

![Den Frosmoth](https://raphgg.github.io/den-bot/data/readme/denfrosmoth.png "Cutie Patootie")

`%pokedex froslass`

![Pokedex Froslass](https://raphgg.github.io/den-bot/data/readme/pokedexfroslass.png "Best Pokèmon Ever Made, Thanks For Coming to My TED Talk.")

## Support & Progress
* [Join](https://discord.gg/ZZU77fz) Alcremie-B's support server to test, get help, and give feedback for the bot!
* [Follow](https://app.gitkraken.com/glo/board/XjQu3nV7egARKaLs) Alcremie-B's progress and updates on its Gitkraken Glo Board!

## Credits
* Many thanks to everyone listed below as without them this bot wouldn't be possible:
- * [Serebii](https://Serebii.net) & [Bulbapedia](https://bulbapedia.bulbagarden.net/) for their mass wealth of Pokémon information and their dedication to host it.
- * [PkParaíso](https://pkparaiso.com) & [Ian Clail](https://www.smogon.com/forums/threads/sun-moon-sprite-project.3577711/) [Layell] for their lovely sprite work on over 1300 different Pokèmon & Forms.
- * [Tax](https://imgur.com/gallery/Tb82GTc) for their awesome gif work on the ball animations.
- * Shirayuki for the bot's profile picture.
- * All of the people over at [Pokémon Raiders](https://discordapp.com/invite/pokemonraiders) for the idea & kindliness.
