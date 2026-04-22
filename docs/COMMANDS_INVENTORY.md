# Discord-OwO-Bot — Complete Command & Alias Inventory

> Auto-generated from source code inspection.
> Source repo: sarifahfirda/Discord-OwO-Bot
> Generation date: 2026-04-22

## Summary
- **Total commands:** 284
- **Total aliases:** 529
- **Categories (13):** `Root`, `Admin / Staff (Gated)`, `Battle`, `Economy`, `Emotes`, `Gamble`, `Meme Generator`, `Patreon / Custom`, `Ranking`, `Shop`, `Social`, `Utilities`, `Zoo / Animals`

## Registration Overview

Commands are registered by `src/commands/command.js` (see `initCommands` at `src/commands/command.js:175`).  That function uses `require-dir` to recursively load every file beneath `src/commands/commandList/`, and for each exported value that is an instance of `CommandInterface` (`src/commands/CommandInterface.js`) it adds the command under each alias.  Files whose export is an array of `CommandInterface` instances (e.g. `patreon/collectible.js`, `patreon/collectibleClasses.js`) are expanded in this inventory as one entry per generated command.

Commands with `owner: true`, `admin: true`, `manager: true`, or `helper: true` are routed to the admin command map and are gated by `src/commands/command.js:86` (`executeAdmin`) — they are only invoked for the bot owner or for staff roles listed in `main.config` and only in configured mod channels.

## Commands by Category

### Utilities

#### `announce`
- **Aliases:** `changelog`, `announcement`, `announcements`
- **Description:** View the latest announcement! Announcements will also be displayed in your daily command! You can disable this by typing 'owo announcement disable'
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/announcement.js:L11`

#### `avatar`
- **Aliases:** `user`
- **Description:** Look at your or other people's avatar!
- **Cooldown:** 2000 ms (2s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/utils/avatar.js:L11`

#### `censor`
- **Aliases:** *(none)*
- **Description:** This will censor any bad words displayed in battle!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/censor.js:L11`

#### `checklist`
- **Aliases:** `task`, `tasks`, `cl`
- **Description:** Get a list of all the things you have left to do!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/utils/checklist.js:L17`

#### `color`
- **Aliases:** `randcolor`, `colour`, `randcolour`
- **Description:** Use the command without any parameters to get a random color! You can also tag a user as an argument to parse prominent colors from their avatar! You can view color roles by adding the text "role" and tagging a user You can also view specific colors with RGB, HEX, or HSL values!
- **Cooldown:** 4000 ms (4s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/color.js:L18`

#### `covid`
- **Aliases:** `cv`, `covid19`, `coronavirus`
- **Description:** Shows the current coronavirus cases. You can specify a country in the arguments. Stay safe out there and please remember to wash your hands. The information is pulled from this github https://www.worldometers.info/coronavirus/
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/covid.js:L16`

#### `disable`
- **Aliases:** *(none)*
- **Description:** Disable a command in the current channel. You can list multiple commands to disable multiple at once. You can also disable a whole group.
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/disable.js:L13`

#### `distorted`
- **Aliases:** `dt`
- **Description:** Check to see if distorted animals are available
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/distored.js:L21`

#### `enable`
- **Aliases:** *(none)*
- **Description:** Enable a command or a command group in the current channel
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/enable.js:L14`

#### `guildlink`
- **Aliases:** *(none)*
- **Description:** Come join our guild! You might be awarded with special gifts once in awhile!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/guildlink.js:L11`

#### `help`
- **Aliases:** *(none)*
- **Description:** This displays the commands or more info on a specific command
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/help.js:L22`

#### `invite`
- **Aliases:** `link`
- **Description:** Want to invite this bot to another server? Use this command!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/invite.js:L11`

#### `math`
- **Aliases:** `calc`, `calculate`
- **Description:** Let me do your math homework! Add an expression for me to solve! More in-depth syntax can be found here: https://mathjs.org/docs/expressions/syntax.html
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/math.js:L16`

#### `patreon`
- **Aliases:** `donate`, `support`, `supporter`
- **Description:** Donate to OwO Bot to help support its growth! Any donations will come with special benefits!
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/patreon.js:L15`

#### `ping`
- **Aliases:** `pong`
- **Description:** Shows the shard latency in ms
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/ping.js:L13`

#### `prefix`
- **Aliases:** *(none)*
- **Description:** Change the prefix for the server! Only Server admins are able to use this command.
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/prefix.js:L29`

#### `rule`
- **Aliases:** `rules`
- **Description:** Display the rules for owo bot!
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/rules.js:L20`

#### `shards`
- **Aliases:** `shard`
- **Description:** *(none)*
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/shard.js:L17`

#### `stats`
- **Aliases:** `stat`, `info`
- **Description:** Some bot stats!
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/stats.js:L12`

#### `suggest`
- **Aliases:** *(none)*
- **Description:** Suggest a new feature. You must be in our support server to suggest.
- **Cooldown:** 600000 ms (600s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/suggest.js:L20`

#### `survey`
- **Aliases:** *(none)*
- **Description:** View the latest survey! Surveys can help us improve the bot.
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/survey.js:L13`

#### `uncensor`
- **Aliases:** *(none)*
- **Description:** This will uncensor any bad words displayed in battle!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/uncensor.js:L11`

#### `vote`
- **Aliases:** *(none)*
- **Description:** Vote on Discord Bot List to gain daily cowoncy!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `utility`
- **Source:** `src/commands/commandList/utils/vote.js:L26`

### Economy

#### `claim`
- **Aliases:** `reward`, `compensation`
- **Description:** Claim rewards! (If there are any c:)
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/economy/claim.js:L13`

#### `cowoncy`
- **Aliases:** `money`, `currency`, `cash`, `credit`, `balance`
- **Description:** Check your cowoncy balance! You can earn more cowoncy through dailies and voting!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/economy/cowoncy.js:L12`

#### `daily`
- **Aliases:** *(none)*
- **Description:** Grab your daily cowoncy every day after 12am PST! Daily streaks will give you extra cowoncy!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/economy/daily.js:L24`

#### `give`
- **Aliases:** `send`
- **Description:** Send some cowoncy to other users! This command must contain a @mention and an amount There is a limit on how much cowoncy you can receive and give.
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/economy/give.js:L20`

#### `quest`
- **Aliases:** `q`
- **Description:** Grab a quest everyday! Complete them to earn rewards! You also have one quest reroll per day! You can earn a new quest after 12am PST
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/economy/quest.js:L20`

### Zoo / Animals

#### `autohunt`
- **Aliases:** `huntbot`, `hb`, `ah`
- **Description:** Use autohunt to hunt for animals automatically! Upgrade huntbot for more efficient hunts!
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/autohunt.js:L22`

#### `hunt`
- **Aliases:** `h`, `catch`
- **Description:** Hunt for some animals for your zoo! Higher ranks are harder to find!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/catch.js:L21`

#### `lootbox`
- **Aliases:** `lb`
- **Description:** Opens a lootbox! Check how many you have in 'owo inv'! You can get some more by hunting for animals. You can get a maximum of 3 lootboxes per day. You can use the items by using 'owo use {id}'
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/lootbox.js:L20`

#### `owodex`
- **Aliases:** `od`, `dex`, `d`
- **Description:** Use the owodex to get information on a pet!
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/owodex.js:L11`

#### `sacrifice`
- **Aliases:** `essence`, `butcher`, `sac`, `sc`
- **Description:** Sacrifice an animal to turn them into animal essence! Animal essence is used to upgrade your huntbot! Sacrificing animals will not prevent you from using them in battle!
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/sacrifice.js:L13`

#### `sell`
- **Aliases:** *(none)*
- **Description:** Sell animals from your zoo! Selling animals will NOT affect your zoo score! You can also sell weapons by their unique weaponID! Selling animals will not prevent you from using them in battle!
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/sell.js:L14`

#### `upgrade`
- **Aliases:** `upg`
- **Description:** Use animal essence to upgrade autohunt! You can specify an amount, upgrade to the next level, or use all your essence.
- **Cooldown:** 1000 ms (1s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/upgrade.js:L28`

#### `zoo`
- **Aliases:** `z`
- **Description:** Displays your zoo! Some animals are rarer than others! Use the 'display' args to display all your animals from your history!
- **Cooldown:** 45000 ms (45s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/zoo/zoo.js:L15`

### Battle

#### `ab`
- **Aliases:** `acceptbattle`
- **Description:** Accept a battle request! If a bet was added, you will have to add the amount to accept it in addition to the battle.
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/ab.js:L13`

#### `battle`
- **Aliases:** `b`, `fight`
- **Description:** *(none)*
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/battle.js:L14`

#### `battlesetting`
- **Aliases:** `bs`, `battlesettings`
- **Description:** *(none)*
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/battleSetting.js:L13`

#### `crate`
- **Aliases:** `weaponcrate`, `wc`
- **Description:** Opens a crate to find weapons!
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/crate.js:L16`

#### `db`
- **Aliases:** `declinebattle`
- **Description:** Decline a battle request!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/db.js:L11`

#### `pets`
- **Aliases:** `pet`
- **Description:** Displays your current pets! Add them by using them in battles!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/pet.js:L14`

#### `rename`
- **Aliases:** *(none)*
- **Description:** Rename an animal from your zoo!
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/rename.js:L11`

#### `team`
- **Aliases:** `squad`, `tm`
- **Description:** Display your team!
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/team.js:L15`

#### `teams`
- **Aliases:** `setteam`, `squads`, `useteams`
- **Description:** Select a different team!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/teams.js:L15`

#### `weapon`
- **Aliases:** `w`, `weapons`, `wep`
- **Description:** *(none)*
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/weapon.js:L16`

#### `weaponshard`
- **Aliases:** `ws`, `weaponshards`, `dismantle`
- **Description:** *(none)*
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/battle/weaponshards.js:L32`

### Shop

#### `buy`
- **Aliases:** *(none)*
- **Description:** Buy an item from the shop!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/shop/buy.js:L15`

#### `describe`
- **Aliases:** `desc`
- **Description:** Describe an item from the shop!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/shop/describe.js:L17`

#### `equip`
- **Aliases:** `use`
- **Description:** Use items from your inventory!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/shop/equip.js:L18`

#### `inventory`
- **Aliases:** `inv`
- **Description:** Displays your inventory! Use 'owo equip' to use them!
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `animals`
- **Source:** `src/commands/commandList/shop/inventory.js:L21`

#### `shop`
- **Aliases:** `market`
- **Description:** Spend your cowoncy for some items!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/shop/shop.js:L26`

#### `trade`
- **Aliases:** `tr`, `gift`
- **Description:** Trade an item with a user!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `economy`
- **Source:** `src/commands/commandList/shop/trade.js:L17`

### Social

#### `acceptmarriage`
- **Aliases:** `am`
- **Description:** Accept a marriage proposal.
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/acceptMarriage.js:L33`

#### `beehive`
- **Aliases:** `hive`, `bh`
- **Description:** Display your pride-ful bees! These bees can only be obtained during certain weeks of pride month.
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/beehive.js:L16`

#### `cookie`
- **Aliases:** `rep`
- **Description:** Give a user a cookie!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/cookie.js:L14`

#### `declinemarriage`
- **Aliases:** `dm`
- **Description:** Decline a marriage proposal.
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/declineMarriage.js:L13`

#### `define`
- **Aliases:** *(none)*
- **Description:** I shall define thy word!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `fun`
- **Source:** `src/commands/commandList/social/define.js:L15`

#### `discordplays`
- **Aliases:** `twitchplays`, `emulator`
- **Description:** *(none)*
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/discordplays.js:L13`

#### `divorce`
- **Aliases:** *(none)*
- **Description:** Escape your marriage
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/divorce.js:L23`

#### `eightball`
- **Aliases:** `8b`, `ask`, `8ball`
- **Description:** Ask a question and get an answer!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `fun`
- **Source:** `src/commands/commandList/social/eightball.js:L80`

#### `emoji`
- **Aliases:** `enlarge`, `jumbo`
- **Description:** Enlarge an emoji! You can list multiple emojis are use the 'previous' keyword to enlarge an emoji from the message above you! You can also steal emojis if you use 'owo emoji setguild'.
- **Cooldown:** 7000 ms (7s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/emoji.js:L14`

#### `level`
- **Aliases:** `lvl`, `levels`, `xp`
- **Description:** Display your Level! Increase your level by talking on Discord! You can gain a maximum of 3000xp per day with a bonus of 500 for the first message of the day! SPAMMING MESSAGES WILL NOT COUNT. You will get rewards for leveling up. If you missed a level up reward, you can type this command to claim it. You can disable level up messages for the guild by using 'owo level disabletext'.
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/level.js:L14`

#### `owo`
- **Aliases:** `owoify`, `ify`
- **Description:** OwOify your text! You can also just type 'owo owoify' to OwOify the message above yours!
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/owoify.js:L14`

#### `pray`
- **Aliases:** `curse`
- **Description:** Pray or curse yourself or other users!!
- **Cooldown:** 300000 ms (300s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/pray.js:L30`

#### `profile`
- **Aliases:** *(none)*
- **Description:** Display your profile! Level up by talking on Discord!
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/profile.js:L13`

#### `propose`
- **Aliases:** `marry`, `marriage`, `wife`, `husband`
- **Description:** Use a ring to marry another user for extra daily rewards! You can reuse the command to upgrade a ring. All rings are the same, there are no extra benefits for a better ring.
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/marry.js:L45`

#### `ship`
- **Aliases:** `combine`
- **Description:** Ships two people!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/ship.js:L13`

#### `translate`
- **Aliases:** `listlang`, `tl`
- **Description:** Translates a message to a specific language. The default language will be english. Use 'owo listlang to list all the languages
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/translate.js:L13`

#### `wallpaper`
- **Aliases:** `wp`, `wallpapers`, `background`, `backgrounds`
- **Description:** View your current wallpapers! Equipped them by clicking the wallpaper emoji. You can buy more wallpapers from the shop.
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `social`
- **Source:** `src/commands/commandList/social/wallpaper.js:L16`

### Ranking

#### `my`
- **Aliases:** `me`, `guild`
- **Description:** Displays your ranking of each category! You can choose you rank within the server or globally! You can also shorten the command like in the example!
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `rankings`
- **Source:** `src/commands/commandList/ranking/me.js:L22`

#### `top`
- **Aliases:** `rank`, `ranking`
- **Description:** Displays the top ranking of each category!
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `rankings`
- **Source:** `src/commands/commandList/ranking/top.js:L22`

### Gamble

#### `blackjack`
- **Aliases:** `bj`, `21`
- **Description:** Gamble your money away in blackjack! You can hit or stand by reacting with emojis! If the command stops responding, retype the command to resume the game!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `gambling`
- **Source:** `src/commands/commandList/gamble/blackjack.js:L20`

#### `coinflip`
- **Aliases:** `cf`, `coin`, `flip`
- **Description:** Flip a coin to earn some cowoncy! You can also shorten the command like in the example!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `gambling`
- **Source:** `src/commands/commandList/gamble/coinflip.js:L19`

#### `drop`
- **Aliases:** `pickup`
- **Description:** This command is now deprecated. ~~Drop some cowoncy in a channel with 'owo drop {amount}'! Users can pick it up with 'owo pickup {amount}' If you try to pick up more than what's on the floor, you'll lose that amount! Be careful!~~
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `gambling`
- **Source:** `src/commands/commandList/gamble/drop.js:L14`

#### `lottery`
- **Aliases:** `bet`, `lotto`
- **Description:** Bet your money in the lottery! The more money you bet, the higher the chance to win! The lottery ends at 12am PST everyday!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `gambling`
- **Source:** `src/commands/commandList/gamble/lottery.js:L13`

#### `slots`
- **Aliases:** `slot`, `s`
- **Description:** Bet your money in the slot machine! Earn up to 10x your money!
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `gambling`
- **Source:** `src/commands/commandList/gamble/slots.js:L24`

### Emotes

#### `blush`
- **Aliases:** `cry`, `dance`, `lewd`, `pout`, `shrug`, `sleepy`, `smile`, `smug`, `thumbsup`, `wag`, `thinking`, `triggered`, `teehee`, `deredere`, `thonking`, `scoff`, `happy`, `thumbs`, `grin`
- **Alias mode:** `distinctAlias` — each alias above resolves to itself (not to `blush`).
- **Description:** Express your emotions!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `emotes`
- **Source:** `src/commands/commandList/emotes/self_emote.js:L16`
- **Note:** Aliases are sourced from src/data/emotes.json → sEmote keys

#### `cuddle`
- **Aliases:** `hug`, `kiss`, `lick`, `nom`, `pat`, `poke`, `slap`, `stare`, `highfive`, `bite`, `greet`, `punch`, `handholding`, `tickle`, `kill`, `hold`, `pats`, `wave`, `boop`, `snuggle`, `fuck`, `sex`
- **Alias mode:** `distinctAlias` — each alias above resolves to itself (not to `cuddle`).
- **Description:** Express your emotions on others!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `actions`
- **Source:** `src/commands/commandList/emotes/user_emote.js:L16`
- **Note:** Aliases are sourced from src/data/emotes.json → uEmote keys

#### `gif`
- **Aliases:** `pic`
- **Description:** Grabs a gif/pic with the given type. To list all the types, type 'owo gif'. Some listed types may not work
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `fun`
- **Source:** `src/commands/commandList/emotes/images.js:L13`

### Meme Generator

#### `communism`
- **Aliases:** `communismcat`
- **Description:** Generate a communism cat meme!
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/communism.js:L13`

#### `distractedbf`
- **Aliases:** `distracted`
- **Description:** Generate a distracted boyfriend meme! Seperate the three arguments with a '\|' bar, or press 'Shift+Enter' between arguments
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/distracted.js:L13`

#### `drake`
- **Aliases:** *(none)*
- **Description:** Generate a Drake meme! Seperate the two arguments with a '\|' bar, or press 'Shift+Enter' between arguments
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/drake.js:L13`

#### `eject`
- **Aliases:** `amongus`
- **Description:** Eject a user into space!
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/eject.js:L15`

#### `emergency`
- **Aliases:** `emergencymeeting`
- **Description:** Call an emergency meeting!
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/emergency.js:L16`

#### `headpat`
- **Aliases:** *(none)*
- **Description:** Create a headpat emoji! You can add it to server if you have used `owo emoji set`
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/headpat.js:L14`

#### `isthisa`
- **Aliases:** *(none)*
- **Description:** Creates a 'is this a ___?' meme! You can also tag a user to use their image!
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/isthisa.js:L15`

#### `slapcar`
- **Aliases:** `slaproof`
- **Description:** Creates a *slaps roof of car* meme! You can also tag a user after your text to use their image instead
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/slapcar.js:L16`

#### `spongebobchicken`
- **Aliases:** `schicken`
- **Description:** Creates a spongebob chicken meme!
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/spongebobchicken.js:L14`

#### `tradeoffer`
- **Aliases:** *(none)*
- **Description:** Generate a Trade Offer meme! Seperate the arguments with a '\|' bar, or press 'Shift+Enter' between arguments
- **Cooldown:** 20000 ms (20s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/tradeoffer.js:L13`

#### `waddle`
- **Aliases:** *(none)*
- **Description:** Create a waddle emoji! You can add it to server if you have used `owo emoji set`
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `memegeneration`
- **Source:** `src/commands/commandList/memegen/waddle.js:L14`

### Patreon / Custom

#### `02kiss`
- **Aliases:** *(none)*
- **Description:** A custom command created by ?611567320552439808?!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/02kiss.js:L13`

#### `alastor`
- **Aliases:** *(none)*
- **Description:** OwO Alastor to show your Alastor! Feed Alastor every day to increase your streak! When Alastor gets upset, offer him a crown to appease him and continue your streak! This command was created by ?229299825072537601?
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/alastor.js:L22`

#### `angel`
- **Aliases:** `agl`
- **Description:** A pair of Angel wings to take you higher than the sky a placed called Heaven. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/angel.js:L28`

#### `army`
- **Aliases:** *(none)*
- **Description:** Collect Army Emblems for your server! You get 15 per day. This command was created by KITSUNE!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/army.js:L19`

#### `babyyoda`
- **Aliases:** *(none)*
- **Description:** Feed baby yoda daily! Give him a silver ball if he throws a fit! This command was created by ?575555630312456193?
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/babyyoda.js:L26`

#### `bat`
- **Aliases:** *(none)*
- **Description:** “I’m batty over you!” This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `bear`
- **Aliases:** *(none)*
- **Description:** Give a bear to someone! You can only gain one if you receive it! This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `bee`
- **Aliases:** `honey`
- **Description:** A busy buzzing bee that loves flowers will bring you sweet honey. Will you will bee mine, I think I've found my honey. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/bee.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/bee.js

#### `bell`
- **Aliases:** `strengthtest`
- **Description:** Step right up! Test your strength in the bell game! This command was created by Geist!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/strengthtest.js:L32`

#### `birthstone`
- **Aliases:** `bstone`, `bsn`
- **Description:** The passage of time is explored through the journey of life. A quest to find the precious gemstones that represents one's birth. Months may pass and possibly a life time to complete. Unlock two hidden gemstones, moonstone & sunstone once you have completed the twelve; Garnet, Amethyst, Aquamarine, Diamond, Emerald, Pearl, Ruby, Peridot, Sapphire, Opal, Citrine, Topaz. This command was created by ?184587051943985152?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/birthstone.js:L97`

#### `blinkbear`
- **Aliases:** *(none)*
- **Description:** Let chill with music K pop Blackpink ❤️ This command was created by ?529452621862273035?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `boba`
- **Aliases:** *(none)*
- **Description:** This custom item can only be given by the owner of this command. This command was created by ?863101441697775616?, and ?473546331689058334?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/boba.js:L26`

#### `bonk`
- **Aliases:** `bomk`
- **Description:** A custom command created by ? ?! Bonk your friends!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `actions`
- **Source:** `src/commands/commandList/patreon/bonk.js:L24`

#### `booger`
- **Aliases:** *(none)*
- **Description:** Receive a naughty kitty named Booger! This command was created by ?665648471340220430?, and ?416987916888440832?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `bully`
- **Aliases:** *(none)*
- **Description:** A custom command created by Geist! Bully your friends!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `actions`
- **Source:** `src/commands/commandList/patreon/bully.js:L29`

#### `bunny`
- **Aliases:** *(none)*
- **Description:** Give a bunny to someone! You can only gain one if you receive it! This command was created by ?370709798020448257?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/bunny.js:L16`

#### `butterfly`
- **Aliases:** `btf`
- **Description:** Leila & Estee A rebirth of an angel, the reincarnation of souls, my love your gentle touch flutters my heart. This command was created by ? ? and ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/butterfly.js:L16`

#### `cake`
- **Aliases:** *(none)*
- **Description:** Give some cake to a friend! You can only gain cake if you receive it! This command was created by [911]Lord
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/cake.js:L17`

#### `calcifer`
- **Aliases:** `calcifer`, `cal`
- **Description:** This command was created by ?665648471340220430?, and ?228381909678292992?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/calcifer.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/calcifer.js

#### `candycane`
- **Aliases:** *(none)*
- **Description:** Give two candy canes to someone! You can only gain one if you receive it! This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/candycane.js:L16`

#### `carlspider`
- **Aliases:** *(none)*
- **Description:** You can only receive this from the owner This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `chicken`
- **Aliases:** `jester`
- **Description:** Give two chickens to someone! You can only gain one if you receive it! This command was created by ? ? and ?428249367577755690?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/chicken.js:L16`

#### `choose`
- **Aliases:** `pick`, `decide`
- **Description:** Let me decide a random option from a list of items! This command was created by PandaDasKissen
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `fun`
- **Source:** `src/commands/commandList/patreon/choose.js:L21`

#### `cloud`
- **Aliases:** *(none)*
- **Description:** Soft mist of cotton gentle and sweet, combine me with thunder and I'll be your worst nightmare. This command was created by ?692146302284202134?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/cloud.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/cloud.js

#### `clover`
- **Aliases:** *(none)*
- **Description:** Send one clover a day and give somebody some luck to start off their day with! &lt;3 This command was created by ?692146302284202134?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `coffee`
- **Aliases:** `java`
- **Description:** Give a coffee to someone! You can only gain coffee if you receive it! This command was created by ❄chocσ˚ℓαtte❄
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/coffee.js:L15`

#### `compliment`
- **Aliases:** `bnice`
- **Description:** Give a compliment to someone! You can only gain one if you receive it! This command was created by ?103409793972043776?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/compliment.js:L16`

#### `corgi`
- **Aliases:** `doggo`
- **Description:** oooo is that a corgi, what a qt whoever gave you that doggo really trusts you "corgi no corgi" This command was created by ?486604819545587723?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `crossfox`
- **Aliases:** `crossfox`, `melanisticfox`
- **Description:** The cross fox is a variant of the red fox which has a long dark stripe running down its back, intersecting another stripe to form a cross over the shoulders. Due to a rare condition called melanism, the commonly red fur comes with some dark stripe. This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/crossfox.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/crossfox.js

#### `crown`
- **Aliases:** *(none)*
- **Description:** Give a crown to someone! You can only gain crown if you receive it! This command was created by crowN
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/crown.js:L15`

#### `cupachicake`
- **Aliases:** `cpc`
- **Description:** Give a cupachicake to someone! You can only gain one if you receive it! This command was created by Beliwolfi
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/cupachicake.js:L15`

#### `curly`
- **Aliases:** *(none)*
- **Description:** Jerome Lester Horwitz, better known by his stage name Curly Howard, was an American comedian and actor. He was well known for his high-pitched voice and vocal expressions ("nyuk-nyuk-nyuk!", "woob-woob-woob!", "soitenly!", "I'm a victim of soikemstance", and barking like a dog. He was the younger brother of Stooges Moe Howard and Shemp Howard. Film critics have cited Curly as the most popular member of the team. His childlike mannerisms and natural comedic charm made him a hit with audiences, particularly children and women. (Combine with moe, shemp, and larry, to make a 3stooges. Use the command: owo curly nyuk.) This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/curly.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/curly.js

#### `darwinsfox`
- **Aliases:** *(none)*
- **Description:** Darwin's Fox (Lycalpoex fulvipes), also known as Zorro Chilote, is an endangered canid. It is not a true fox. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/darwinsfox.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/darwinsfox.js

#### `dayang3`
- **Aliases:** `dayang`, `cinta`, `indonesia`
- **Description:** Hallo...!! I am dayang🌷 from Indonesia When you have 𝖈𝖎𝖓𝖙𝖆, 𝖐𝖆𝖘𝖎𝖍 and 𝖘𝖆𝖞𝖆𝖓𝖌, you can get my 𝖇𝖚𝖓𝖌𝖆 as a present from me...♡ ♧ OwOd cinta ♧ OwOd kasih ♧ OwOd sayang ♧ ♧ find me in .gg/owobot & .gg/hns This command was created by ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/dayang.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/dayang.js

#### `death`
- **Aliases:** *(none)*
- **Description:** These collectables are only given out by ? ?. This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/death.js:L15`

#### `des`
- **Aliases:** `kasih`
- **Description:** Dire Exchange Service ツ is a growing community revolved around gaming bots such as OwO, AniGame, Karuta and many more; and it is a place for all to grind. This command was created by .greywolf., direthedire, and dayang. This command was created by ?384202884553768961?, ?707939636835516457?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `devil`
- **Aliases:** `dvl`
- **Description:** A pair of Devil wings to take you to the underworld a place called Hell. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/devil.js:L27`

#### `dg-hug`
- **Aliases:** `sayang`
- **Description:** A hug is meant to show someone you care and that you are there for them. Always keep the spirit up; life is short - enjoy life to the fullest. This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `dhole`
- **Aliases:** *(none)*
- **Description:** Dhole (Cuon alpinus), also known as Asian wild dog, Asiatic wild dog, Indian wild dog, whistling dog, red dog, and mountain wolf. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/dhole.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/dhole.js

#### `dish`
- **Aliases:** *(none)*
- **Description:** Give a dish to someone! You can only gain one if you receive it! This command was created by 👑𝕮𝖗𝖔𝖜𝖓👑
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/dish.js:L14`

#### `doll`
- **Aliases:** *(none)*
- **Description:** Give a headless doll to a friend! This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `donut`
- **Aliases:** *(none)*
- **Description:** Give donuts to someone! You can only gain one if you receive it! This command was created by ?575555630312456193?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/donut.js:L16`

#### `dragon`
- **Aliases:** `dgn`
- **Description:** These collectables are only given out by ? ? and ? ?. This command was created by ? ? and ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/dragon.js:L16`

#### `dtn`
- **Aliases:** `destiny`
- **Description:** Destined to cross paths but never to meet. In this lifetime, I loved your soul before I could touch you. Unable to change this time line, where we're not destined to complete our love story. In this lifetime, this destiny, you're my last love, my one and only love. But these promises are just sweet lies therefore, I owe you and will love you onto the next life to complete our story. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/destiny.js:L36`

#### `duwasvivu`
- **Aliases:** *(none)*
- **Description:** This command was created by ?666840617380478977?
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/duwasvivu.js:L11`

#### `egg`
- **Aliases:** *(none)*
- **Description:** Here, have an egg! use wisely.... This command was created by ?204118895106195456?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `ewolf`
- **Aliases:** *(none)*
- **Description:** Ethiopian wolf, also known as the Simien jackal or Simien fox. It is one of the world's rarest canids; there are less than 500 Ethiopian wolves left in the world. The Ethiopian wolf has been considered rare since it was first recorded scientifically in 1835. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `fate`
- **Aliases:** *(none)*
- **Description:** This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/fate.js:L22`

#### `fear`
- **Aliases:** `nommy`
- **Description:** What do you fear? fears can alarming, but we all overcome them... unless it's me noming you I'd nom you if I could\" This command was created by ?486604819545587723?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/fear.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/fear.js

#### `flame`
- **Aliases:** `flm`
- **Description:** From the deepest depths of the underworld comes a flame like no other. Do not be fooled by its beauty, although it shines like the ocean blue. One touch and your soul will leave you eternally. *dedicated/inspired by macchiato and estee* This command was created by ?640563808884228126?, ?863101441697775616?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `friend`
- **Aliases:** *(none)*
- **Description:** A friend is someone who is always there for you in the good times and the bad. A friend is loyal. A friend will never judge you and always accepts you for who you are. The word "friend" comes from Old English "frēond", which means "to love" and "to honor". REQUIREMENT to receive is to show kindness to other OwO players. This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `frogegg`
- **Aliases:** *(none)*
- **Description:** Give a frog egg to someone! Once you collect 6, they will be changed into a silver ball. This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/frogEgg.js:L17`

#### `galikat`
- **Aliases:** *(none)*
- **Description:** All aboard the unsinkable cake haven, the HMS GaliKat. The SHIP that launched a thousand owos…..! This command was created by ?665648471340220430?, ?416987916888440832?, and ?710674986863427634?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `gauntlet`
- **Aliases:** *(none)*
- **Description:** Combine 1 yinyangs to create a thanos gauntlet! Snap to choose one of 3 events! This command was created by ! 「陰陽」 Kitsune ☯
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/gauntlet.js:L18`

#### `genie`
- **Aliases:** *(none)*
- **Description:** This custom item can only be given by the owner of this command. This command was created by ?863101441697775616?, and ?667180052592721941?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/genie.js:L26`

#### `ghost`
- **Aliases:** *(none)*
- **Description:** “Boo! Did I scare you?” This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `ginseng`
- **Aliases:** *(none)*
- **Description:** Give two ginsengs to someone! You can only gain one if you receive it! Ginseng is the root of plants in the genus Panax, characterized by the presence of ginsenosides and gintonin, notable for its healing properties. One of the first written texts covering the use of ginseng as a medicinal herb was written in China in 196 AD. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `goldenegg`
- **Aliases:** *(none)*
- **Description:** These collectables are only given out by ? ?. This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/goldenegg.js:L15`

#### `grim`
- **Aliases:** *(none)*
- **Description:** A custom command created by ?926910724939333632?!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/grim.js:L11`

#### `grizzly`
- **Aliases:** *(none)*
- **Description:** Give two grizzleys to someone! You can only gain one if you receive it! This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `guillotine`
- **Aliases:** *(none)*
- **Description:** A custom command created by ?665648471340220430?!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `actions`
- **Source:** `src/commands/commandList/patreon/guillotine.js:L17`

#### `hauntedhouse`
- **Aliases:** *(none)*
- **Description:** Combine a ghost, witch, bat, and a spider to create a haunted house. This command was created by ?665648471340220430?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/hauntedhouse.js:L14`

#### `icecream`
- **Aliases:** *(none)*
- **Description:** Give an ice cream to someone! You can only gain ice cream if you receive it! This command was created by Łord
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/icecream.js:L24`

#### `kfire`
- **Aliases:** *(none)*
- **Description:** K-fire server is a server that made by Kurdistan. This server is a place for you to play some bot games such as OwO, Anigame, Tatsu, etc. This collectible is only given out by the creators. Nobody else can give it This command was created by ?759412813617430619?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `king`
- **Aliases:** *(none)*
- **Description:** A noble descendant of God, a royal ruler over mankind. Behind ever King is a powerful Queen. The king of spades x "Guards take him away!" This command was created by ?282666590565171210?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/king.js:L27`

#### `kitty`
- **Aliases:** *(none)*
- **Description:** A litte sweet cuddly fur ball to snuggle up with. This command was created by ?460987842961866762?, and ?777641801212493826?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/kitty.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/kitty.js

#### `koi`
- **Aliases:** `koi`, `lotus`
- **Description:** Happy OwO Anniversary and many more to come. Our friendship is beautiful and we balance like the Yin & Yang just like the two koi fish representing the duality of life. This command was created by ?460987842961866762?, and ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/koi.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/koi.js

#### `larry`
- **Aliases:** *(none)*
- **Description:** Louis Feinberg, better known by his stage name Larry Fine, was an American comedian, actor, and musician. In his early childhood, Fine's arm was accidentally burned with acid that his father used to test jewelry for its gold content. Fine's parents later gave him violin lessons to help strengthen the damaged muscles in his forearm. He became so proficient in it that his parents wanted to send him to a European music conservatory, but the plan was thwarted by the outbreak of World War I. To further strengthen his damaged arm, Fine took up boxing in his teens, winning one professional bout. (Combine with moe, shemp, and curly to make a 3stooges. See the curly help for more info.) This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/larry.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/larry.js

#### `latte`
- **Aliases:** *(none)*
- **Description:** This custom item can only be given by the owner of this command. This command was created by ?863101441697775616?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/latte.js:L26`

#### `lemon`
- **Aliases:** `lemonade`, `lmn`
- **Description:** When life gives you lemons, ill give you lemon-aid. Lemon tell ya, the zest chance to get lemons is through quest help. Owo lemon squeeze to make your refreshing lemonade. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/lemon.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/lemon.js

#### `life`
- **Aliases:** *(none)*
- **Description:** These collectables are only given out by ? ?. This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/life.js:L15`

#### `lilbee`
- **Aliases:** `lilbee`
- **Description:** Created by Lil and Bee to celebrate 1000 days of Owo marriage! This command was created by ?635873165758824449?, and ?423166705477353472?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/lilbee.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/lilbee.js

#### `lollipop`
- **Aliases:** *(none)*
- **Description:** Give a lollipop to someone! You can only gain one if you receive it! This command was created by SleepyPanda
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/lollipop.js:L16`

#### `love`
- **Aliases:** *(none)*
- **Description:** Give love to someone! Collect 5 to combine them into a heart master! You can only gain love if you receive it! This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/love.js:L15`

#### `lovenote`
- **Aliases:** `ln`
- **Description:** Receive both halves of the two love notes to complete your love letter. This command was created by ?692146302284202134?, and ?160095846703038466?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/lovenote.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/lovenote.js

#### `luv`
- **Aliases:** `luv`, `lovey`
- **Description:** everybody knows something I don't and I wonder how to keep a good thing going "there was a time I would die just to be who you liked" ps: a special thank you to A I E D, xnurag, and gamer for the percentage rates ;) This command was created by ?486604819545587723?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/luv.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/luv.js

#### `lxv`
- **Aliases:** *(none)*
- **Description:** Make sure to give Hedge some love, and he might bring you a gift! Only given out in lovesick. A server for OwO, anigame and ERPG grinders! .gg/lxv This command was created by ?412812867348463636?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/lxv.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/lxv.js

#### `magic`
- **Aliases:** *(none)*
- **Description:** Give some Black Magic to a friend! This command was created by ?145541256779530240?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/magic.js:L27`

#### `magoo`
- **Aliases:** *(none)*
- **Description:** Mr. Magoo is a fictional cartoon character voiced by Jim Backus. Mr. Magoo is a wealthy elderly retiree who gets into comical situations as a result of his extreme near-sightedness, compounded by his stubborn refusal to admit the problem. This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/magoo.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/magoo.js

#### `martini`
- **Aliases:** *(none)*
- **Description:** Give a martini to a friend! This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `meshi`
- **Aliases:** *(none)*
- **Description:** Give some meshi to someone! Collect 6 to combine them into badges! You can only gain meshi if you receive it! This command was created by ?403989717483257877?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/meshi.js:L15`

#### `milk`
- **Aliases:** *(none)*
- **Description:** Give a glass of milk to someone! You can only gain one if you receive it! This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/milk.js:L16`

#### `mochi`
- **Aliases:** *(none)*
- **Description:** A bite size delectable snack you can’t live without. As sweet as pie, as cold as the winters breeze, nothing compares to my mochi. This command was created by ?863101441697775616?, and ?282666590565171210?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/mochi.js:L28`

#### `moe`
- **Aliases:** *(none)*
- **Description:** Moses Harry Horwitz, better known by his stage name Moe Howard, was an American comedian and actor. He is best known as the leader of the Three Stooges. He loved to read, as his older brother Jack recalled: "I had many Horatio Alger books, and it was Moe's greatest pleasure to read them. This helped him in his acting career; he could memorize his lines quickly and easily. (Combine with shemp, larry, and curly to make a 3stooges. See the curly help for more info.) This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/moe.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/moe.js

#### `moon`
- **Aliases:** *(none)*
- **Description:** I miss you like the moon misses the sun, forever separated by thousands of miles for thousands of years. Destined to chase it until the end of time. The sun and moon misses each other without any hope of meeting ever. Love by the moon This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/moon.js:L28`

#### `music`
- **Aliases:** `msc`
- **Description:** ♪♫ I wish you were here to compose another melody, I promise when I'm missing you, I'll play our symphony, You are my melody and I am your symphony ♬♩ This command was created by ?578335497793961993?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `nier`
- **Aliases:** *(none)*
- **Description:** Plug-in Chips are items that you can acquire for Skills. Enjoy it. This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/nier.js:L15`

#### `obw`
- **Aliases:** *(none)*
- **Description:** These collectables are only given out by ?443015921968349184?. This command was created by ?443015921968349184? https://owobot.fandom.com
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/obw.js:L15`

#### `obwspecial`
- **Aliases:** `appreciate`
- **Description:** Exclusive collectible created for the OBW community on the collaboration with amazing OwO Bot Wiki discord members. Special thanks to Sliverme, Frosty_, Pandaddy, tinsetia, StunDra, Blue, Max Verstappen fan, dayang🌷, greywolf, jean., Amada, Mal., Radiohead, Xctroy, NarutoUzumaki, theraremixedchick, Ajea, ibot, Mrukia and everyone else who contributed This command was created by ?466629903434121228?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `painteddog`
- **Aliases:** `painted-dog`
- **Description:** African wild dog (Lycaon pictus), also called painted dog, and cape hunting dog. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/painteddog.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/painteddog.js

#### `pancakes`
- **Aliases:** *(none)*
- **Description:** Give a pancake to someone! You can only gain one if you receive it! This command was created by ?665648471340220430?, and ?710674986863427634?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `panda`
- **Aliases:** *(none)*
- **Description:** Give two pandas to someone! You can only gain one if you receive it! This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `penguin`
- **Aliases:** `pgn`
- **Description:** Aptenodytes, a King penguin waddling the ice lands. A great rock collector to woo and gift you. As penguins mate for life, He can't fly away and will swim great oceans for you. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `pika`
- **Aliases:** `pikapika`
- **Description:** Pikachuuuuuu! This command was created by ?693470720281280532?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/pika.js:L11`

#### `pikachu`
- **Aliases:** `pikachu`, `chu`
- **Description:** Charmeleons are red, Wartortles are blue, If you catch my heart, I’ll be your pikachu This command was created by ?768465041489657867?, ?968621197011062804?, ?879313703990870047?, and ?969176350621589514?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/pikachu.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/pikachu.js

#### `piku`
- **Aliases:** *(none)*
- **Description:** Pick one PikPik carrot. Each day you can only do this command one more time than the amount of times you did it the day before. This command was created by ?245103025805328384?
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/piku.js:L17`

#### `pizza`
- **Aliases:** *(none)*
- **Description:** Give a pizza to someone! You can only gain pizza if you receive it! This command was created by Cosmonaut
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/pizza.js:L15`

#### `planet`
- **Aliases:** *(none)*
- **Description:** Explore the galaxy and find all 9 planets, unless you get unlucky and collect some space rocks instead.. or a secret companion to keep you company on your space ship! This collectible can only be given out by ?692146302284202134? & ?412812867348463636?
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/planet.js:L75`

#### `poison`
- **Aliases:** *(none)*
- **Description:** Love could be labeled poison and we'd drink it anyways. Subcommands: owo poison mix This command was created by ?665417324949405706?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/poison.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/poison.js

#### `poutine`
- **Aliases:** *(none)*
- **Description:** Give a poutine to someone! You can only gain poutine if you receive it! This command was created by Mr.Poutine
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/poutine.js:L24`

#### `puppy`
- **Aliases:** `pup`
- **Description:** Pick one up a puppy. Each day you can only do this command one more time than the amount of times you did it the day before. This command was created by ?575555630312456193?
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/puppy.js:L14`

#### `queen`
- **Aliases:** *(none)*
- **Description:** A noble descendant of God, a royal ruler over mankind. Treat her like a queen and she\'ll treat you like a king. The queen of hearts x "Off with your head!" This command was created by ?282666590565171210?, and ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/queen.js:L27`

#### `rainbow`
- **Aliases:** `raindrop`, `wet`, `rain`
- **Description:** May Happiness Rain On You! May Your Sorrows Be Washed Away In The Rain… Sometimes, If You Want The Rainbow, You Gotta Put Up With The Rain! Collect 8 Raindrops to get a Rainbow! This command can only be given out by ?578335497793961993?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/rain.js:L42`

#### `redenvelope`
- **Aliases:** `hongbao`, `angpow`
- **Description:** Red envelope is small red and gold packets, containing money as a symbol of good luck. Collect 8 Red Envelopes to get a Gold! This command was created by ?605994815317999635?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/redenvelope.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/redenvelope.js

#### `redwolf`
- **Aliases:** *(none)*
- **Description:** The Red Wolf is the rarest and most endangered of all the wolf species, with less than 20 individuals left in the wild. It is listed as a Critically Endangered species, facing an extremely high risk of extinction in the wild. Extinction is generally considered to be the death of the last individual of the species. Today the only place red wolves can be found in the wild is in eastern North Carolina's Albemarle Peninsula. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `regret`
- **Aliases:** *(none)*
- **Description:** "same fears, same dreams" This command was created by ?486604819545587723?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/regret.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/regret.js

#### `roll`
- **Aliases:** `d20`
- **Description:** Roll a N-sided die! This command was created by Gut Funk!
- **Cooldown:** 5000 ms (5s)
- **Access:** Public
- **Group(s):** `fun`
- **Source:** `src/commands/commandList/patreon/dice.js:L28`

#### `rose`
- **Aliases:** `bouquet`
- **Description:** Give a rose to someone! You can only gain one if you receive it! 5 roses will become a bouquet. This command was created by ?370709798020448257?
- **Cooldown:** 3000 ms (3s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/rose.js:L17`

#### `rum`
- **Aliases:** *(none)*
- **Description:** Give a tankards of rum to someone! You can only gain one if you receive it! This command was created by Healoholic
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/rum.js:L14`

#### `run`
- **Aliases:** *(none)*
- **Description:** Run one kilometer. Each day you can only do this command one more time than the amount of times you did it the day before. This command was created by ?103409793972043776?
- **Cooldown:** 60000 ms (60s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/run.js:L14`

#### `sakura`
- **Aliases:** *(none)*
- **Description:** These collectables are only given out by ? ?. This command was created by ? ?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/sakura.js:L15`

#### `sammy`
- **Aliases:** *(none)*
- **Description:** Sammy is a Biewer Terrier. The Biewer Terrier is an elegant, longhaired, tri-colored terrier whose only purpose in life is to love and be loved. The Biewer was developed thru selective breeding of the Yorkshire Terrier to highlight the recessive piebald gene (to draw out the white color). The Biewer is a very hearty, athletic dog and an excellent hunter of vermin. They are lighthearted, have a childlike attitude and like to carry toys in their mouths. Biewers average 10" tall, weighing around 5 pounds, and live about 16 years. This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `saturn`
- **Aliases:** *(none)*
- **Description:** Send a saturn to someone! This command was created by ?856036736970260490?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `sharingan`
- **Aliases:** *(none)*
- **Description:** Only the owner can send this item. This command was created by Rikudou Sennin
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/sharingan.js:L14`

#### `shemp`
- **Aliases:** *(none)*
- **Description:** Samuel Horwitz, better known by his stage name Shemp Howard, was an American comedian and actor. He was called "Shemp" because "Sam" came out that way in his mother's thick Litvak accent. He is best known as the third Stooge in the Three Stooges, a role he played when the act began in the early 1920s, and again in 1946 to replace his brother Curly as the third Stooge after Curly's illness. (Combine with moe, larry, and curly to make a 3stooges. See the curly help for more info.) This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/shemp.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/shemp.js

#### `shifu`
- **Aliases:** `ufo`, `catto`
- **Description:** Hopefully these fluffy cattos make your day brighter! These collectibles are only given out by ?412812867348463636?, ?692146302284202134? and ?606142158067597332? This command was created by ?412812867348463636?, ?692146302284202134?, and ?606142158067597332?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/catto.js:L51`

#### `shootingstar`
- **Aliases:** `shootingstar`, `ss`
- **Description:** Give out a shooting star! Merge two shooting stars with \`owo shootingstar unite\`! This command was created by ?370709798020448257?, ?412812867348463636?, ?692146302284202134?, ?417214768970203136?, and ?606142158067597332?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/shootingstar.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/shootingstar.js

#### `slime`
- **Aliases:** *(none)*
- **Description:** Give a slime to someone! You can only gain one if you receive it! This command was created by ?403989717483257877?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/slime.js:L16`

#### `smokeheart`
- **Aliases:** `heart`
- **Description:** Give two smoke hearts to someone! You can only gain one if you receive it! This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `snake`
- **Aliases:** *(none)*
- **Description:** Give snakes to someone! This command was created by ?380822909813391360?, and ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/snake.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/snake.js

#### `snowball`
- **Aliases:** *(none)*
- **Description:** Give a snowball to someone! Collect 5 to combine them into a snowman! You can only gain snowballs if you receive it! This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/snowball.js:L15`

#### `sonic`
- **Aliases:** *(none)*
- **Description:** Give two sonics to someone! You can only gain one if you receive it! This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `sootsprite`
- **Aliases:** `soot`, `sootgremlin`, `susuwatari`
- **Description:** Normally you can’t see Soot Gremlins. But every once in awhile when you go from a bright place to a dark one, you can catch a glimpse of them…. This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `spider`
- **Aliases:** *(none)*
- **Description:** Send a spider to a friend! This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `star`
- **Aliases:** *(none)*
- **Description:** Star light, Star bright. First star I see tonight I wish I may, I wish I might. Have the wish, I wish tonight. This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `stitch`
- **Aliases:** *(none)*
- **Description:** Lilo says that "ohana means family, family means nobody gets left behind or forgotten". I hope this little alien starts to be part of your family now! This command was created by ?942100445105647686?, and ?638420840765063178?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/stitch.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/stitch.js

#### `sun`
- **Aliases:** *(none)*
- **Description:** I love you like the sun loves the moon, forever separated by thousands of miles for thousands of years. He died every night just to let her breathe. The sun and moon love each other without any hope of meeting ever. Live by the sun This command was created by ?460987842961866762?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/sun.js:L28`

#### `sunflower`
- **Aliases:** *(none)*
- **Description:** Give sunflowers to someone! You can only gain one if you receive it! This command was created by ?541103499992367115?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/sunflower.js:L15`

#### `taco`
- **Aliases:** *(none)*
- **Description:** Give a taco to someone! You can only gain one if you receive it! This command was created by ?575555630312456193?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/taco.js:L16`

#### `tarot`
- **Aliases:** *(none)*
- **Description:** Ask a question and answer them with tarot cards! This command was created by ?250383887312748545?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/tarot.js:L74`

#### `teddy`
- **Aliases:** *(none)*
- **Description:** Give two teddy bears to someone! You can only gain one if you receive it! This command was created by ?625340848556474369?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `tequila`
- **Aliases:** *(none)*
- **Description:** This item can only be given out by the creator. This command was created by ?427296171883626496?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/tequila.js:L35`

#### `totoro`
- **Aliases:** *(none)*
- **Description:** "Try Laughing. Then Whatever Scares You Will Go Away”. We hope this Forest Spirit never lets you feel alone! This command was created by ?777641801212493826?, ?193140307326402562?, and ?942100445105647686?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/totoro.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/totoro.js

#### `truthordare`
- **Aliases:** `td`
- **Description:** Send someone a Truth or Dare! Including an optional @mention for a direct truth/dare or no @mention. Specifying either a truth or dare, or no type for either a truth or dare at random This command was created by ?442112392868921365?!
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/truthordare.js:L96`

#### `turnip`
- **Aliases:** *(none)*
- **Description:** Turnips are the lifeblood of the Nook family Fortune, if you would like one you must find it's creator ?owner?. This command was created by ?145541256779530240?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/turnip.js:L27`

#### `unicorn`
- **Aliases:** *(none)*
- **Description:** The unicorn is a legendary creature with a single large, pointed, spiraling horn projecting from its forehead. This command was created by ?384202884553768961?, and ?778204442411008021?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/unicorn.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/unicorn.js

#### `vert`
- **Aliases:** *(none)*
- **Description:** Send a vert to someone! This command was created by ?963635559266390066?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectibleClasses.js:L25`
- **Collectible class:** `src/commands/commandList/patreon/collectibles/vert.js`
- **Note:** Generated from src/commands/commandList/patreon/collectibles/vert.js

#### `water`
- **Aliases:** *(none)*
- **Description:** Give two cups of water to someone! You can only gain one if you receive it! This command was created by ? ?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/water.js:L17`

#### `witch`
- **Aliases:** *(none)*
- **Description:** “Double, double toil and trouble; fire burn and cauldron bubble!” This command was created by ?665648471340220430?
- **Cooldown:** 15000 ms (15s)
- **Access:** 🔒 Patreon Owner Only (giving)
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `wolf`
- **Aliases:** *(none)*
- **Description:** Give a wolf to a friend! This command was created by ?384202884553768961?
- **Cooldown:** 15000 ms (15s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/collectible.js:L258`
- **Note:** Generated per entry in src/commands/commandList/patreon/utils/collectibles.json

#### `yinyang`
- **Aliases:** `yy`
- **Description:** Give a yin and yang to someone! Collect 6 to combine them into ramen! You can only gain ying yangs if you receive it! This command was created by ! 「陰陽」 Kitsune ☯
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/yinyang.js:L15`

#### `zodiackey`
- **Aliases:** `zk`
- **Description:** Give a zodiac key to someone! You can only gain one if you receive it! There are 12 in total to collect: Aquarius, Pisces, Aries, Taurus, Gemini, Cancer, Leo, Virgo, Libra, Scorpio, Sagittarius and Capricorn. This command was created by ?707939636835516457?
- **Cooldown:** 30000 ms (30s)
- **Access:** Public
- **Group(s):** `patreon`
- **Source:** `src/commands/commandList/patreon/zodiackey.js:L68`

### Admin / Staff (Gated)

#### `addallcustomize`
- **Aliases:** `aac`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addAllCustomize.js:L14`

#### `addallweapons`
- **Aliases:** `aaw`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addAllWeapons.js:L12`

#### `addannouncement`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addAnnouncement.js:L11`

#### `addbattle`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addBattle.js:L14`

#### `addcookie`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addCookie.js:L14`

#### `addcowoncy`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addCowoncy.js:L14`

#### `adddaily`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addDaily.js:L14`

#### `addgive`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addGive.js:L14`

#### `addhunt`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addHunt.js:L14`

#### `addinventory`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addInventory.js:L14`

#### `addpatreon`
- **Aliases:** `addpatreons`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addPatreon.js:L14`

#### `addpet`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addPet.js:L11`

#### `addpray`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addPray.js:L14`

#### `addweapon`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addWeapon.js:L14`

#### `addzoo`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/addZoo.js:L14`

#### `adminprofile`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/adminProfile.js:L13`

#### `ban`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/ban.js:L13`

#### `bancommand`
- **Aliases:** `bc`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/banCommand.js:L13`

#### `banguildmembers`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/banGuildMembers.js:L11`

#### `banstatus`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/banstatus.js:L11`

#### `broadcasteval`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/broadcastEval.js:L11`

#### `captcha`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/captcha.js:L18`

#### `cg`
- **Aliases:** `creategiveaway`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/creategiveaway.js:L11`

#### `custompet`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/customPet.js:L47`

#### `deleteuser`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/deleteUser.js:L11`

#### `disablecaptcha`
- **Aliases:** `enablecaptcha`, `setcaptcha`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/disableCaptcha.js:L11`

#### `echo`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/echo.js:L11`

#### `eval`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/eval.js:L11`

#### `getpatreons`
- **Aliases:** `distributecowoncy`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/getPatreonRewards.js:L22`

#### `giveall`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/giveall.js:L11`

#### `givecustompetticket`
- **Aliases:** `gcpt`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/giveCustomPetTicket.js:L11`

#### `givegiveawayticket`
- **Aliases:** `ggt`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/giveGiveawayTicket.js:L11`

#### `giveperkticket`
- **Aliases:** `giveticket`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/givePerkTicket.js:L11`

#### `lift`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/lift.js:L11`

#### `liftcommand`
- **Aliases:** `lc`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/liftCommand.js:L13`

#### `msgusers`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/msgUsers.js:L11`

#### `pausebot`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/pauseBot.js:L11`

#### `prayfrom`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/prayfrom.js:L22`

#### `prayto`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/prayto.js:L22`

#### `refreshanimals`
- **Aliases:** `ra`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/refreshAnimals.js:L11`

#### `removeoptout`
- **Aliases:** `roo`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/removeOptOut.js:L11`

#### `removestrike`
- **Aliases:** `setstrike`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/removeStrike.js:L11`

#### `reply`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/reply.js:L11`

#### `resetbot`
- **Aliases:** `restartbot`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/resetbot.js:L11`

#### `resetcowoncy`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/resetCowoncy.js:L11`

#### `resetowo`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/resetOwo.js:L11`

#### `sendverif`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/sendverif.js:L13`

#### `testevent`
- **Aliases:** `te`
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/testEvent.js:L11`

#### `transaction`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/transaction.js:L22`

#### `warn`
- **Aliases:** *(none)*
- **Description:** *(none)*
- **Cooldown:** N/A
- **Access:** 🔒 Owner Only
- **Source:** `src/commands/commandList/admin/warn.js:L11`

### Root

#### `points`
- **Aliases:** *(none)*
- **Description:** Gives the user a point. This is the same as just saying owo in your messages. You weren't really suppose to find this.
- **Cooldown:** 10000 ms (10s)
- **Access:** Public
- **Source:** `src/commands/commandList/points.js:L11`

## Appendix A — Alphabetical Alias Lookup Table

| Alias | Resolves to | Source |
|-------|-------------|--------|
| `02kiss` | `02kiss` | `src/commands/commandList/patreon/02kiss.js:L13` |
| `21` | `blackjack` | `src/commands/commandList/gamble/blackjack.js:L20` |
| `8b` | `eightball` | `src/commands/commandList/social/eightball.js:L80` |
| `8ball` | `eightball` | `src/commands/commandList/social/eightball.js:L80` |
| `aac` | `addallcustomize` | `src/commands/commandList/admin/addAllCustomize.js:L14` |
| `aaw` | `addallweapons` | `src/commands/commandList/admin/addAllWeapons.js:L12` |
| `ab` | `ab` | `src/commands/commandList/battle/ab.js:L13` |
| `acceptbattle` | `ab` | `src/commands/commandList/battle/ab.js:L13` |
| `acceptmarriage` | `acceptmarriage` | `src/commands/commandList/social/acceptMarriage.js:L33` |
| `addallcustomize` | `addallcustomize` | `src/commands/commandList/admin/addAllCustomize.js:L14` |
| `addallweapons` | `addallweapons` | `src/commands/commandList/admin/addAllWeapons.js:L12` |
| `addannouncement` | `addannouncement` | `src/commands/commandList/admin/addAnnouncement.js:L11` |
| `addbattle` | `addbattle` | `src/commands/commandList/admin/addBattle.js:L14` |
| `addcookie` | `addcookie` | `src/commands/commandList/admin/addCookie.js:L14` |
| `addcowoncy` | `addcowoncy` | `src/commands/commandList/admin/addCowoncy.js:L14` |
| `adddaily` | `adddaily` | `src/commands/commandList/admin/addDaily.js:L14` |
| `addgive` | `addgive` | `src/commands/commandList/admin/addGive.js:L14` |
| `addhunt` | `addhunt` | `src/commands/commandList/admin/addHunt.js:L14` |
| `addinventory` | `addinventory` | `src/commands/commandList/admin/addInventory.js:L14` |
| `addpatreon` | `addpatreon` | `src/commands/commandList/admin/addPatreon.js:L14` |
| `addpatreons` | `addpatreon` | `src/commands/commandList/admin/addPatreon.js:L14` |
| `addpet` | `addpet` | `src/commands/commandList/admin/addPet.js:L11` |
| `addpray` | `addpray` | `src/commands/commandList/admin/addPray.js:L14` |
| `addweapon` | `addweapon` | `src/commands/commandList/admin/addWeapon.js:L14` |
| `addzoo` | `addzoo` | `src/commands/commandList/admin/addZoo.js:L14` |
| `adminprofile` | `adminprofile` | `src/commands/commandList/admin/adminProfile.js:L13` |
| `agl` | `angel` | `src/commands/commandList/patreon/angel.js:L28` |
| `ah` | `autohunt` | `src/commands/commandList/zoo/autohunt.js:L22` |
| `alastor` | `alastor` | `src/commands/commandList/patreon/alastor.js:L22` |
| `am` | `acceptmarriage` | `src/commands/commandList/social/acceptMarriage.js:L33` |
| `amongus` | `eject` | `src/commands/commandList/memegen/eject.js:L15` |
| `angel` | `angel` | `src/commands/commandList/patreon/angel.js:L28` |
| `angpow` | `redenvelope` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `announce` | `announce` | `src/commands/commandList/utils/announcement.js:L11` |
| `announcement` | `announce` | `src/commands/commandList/utils/announcement.js:L11` |
| `announcements` | `announce` | `src/commands/commandList/utils/announcement.js:L11` |
| `appreciate` | `obwspecial` | `src/commands/commandList/patreon/collectible.js:L258` |
| `army` | `army` | `src/commands/commandList/patreon/army.js:L19` |
| `ask` | `eightball` | `src/commands/commandList/social/eightball.js:L80` |
| `autohunt` | `autohunt` | `src/commands/commandList/zoo/autohunt.js:L22` |
| `avatar` | `avatar` | `src/commands/commandList/utils/avatar.js:L11` |
| `b` | `battle` | `src/commands/commandList/battle/battle.js:L14` |
| `babyyoda` | `babyyoda` | `src/commands/commandList/patreon/babyyoda.js:L26` |
| `background` | `wallpaper` | `src/commands/commandList/social/wallpaper.js:L16` |
| `backgrounds` | `wallpaper` | `src/commands/commandList/social/wallpaper.js:L16` |
| `balance` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `ban` | `ban` | `src/commands/commandList/admin/ban.js:L13` |
| `bancommand` | `bancommand` | `src/commands/commandList/admin/banCommand.js:L13` |
| `banguildmembers` | `banguildmembers` | `src/commands/commandList/admin/banGuildMembers.js:L11` |
| `banstatus` | `banstatus` | `src/commands/commandList/admin/banstatus.js:L11` |
| `bat` | `bat` | `src/commands/commandList/patreon/collectible.js:L258` |
| `battle` | `battle` | `src/commands/commandList/battle/battle.js:L14` |
| `battlesetting` | `battlesetting` | `src/commands/commandList/battle/battleSetting.js:L13` |
| `battlesettings` | `battlesetting` | `src/commands/commandList/battle/battleSetting.js:L13` |
| `bc` | `bancommand` | `src/commands/commandList/admin/banCommand.js:L13` |
| `bear` | `bear` | `src/commands/commandList/patreon/collectible.js:L258` |
| `bee` | `bee` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `beehive` | `beehive` | `src/commands/commandList/social/beehive.js:L16` |
| `bell` | `bell` | `src/commands/commandList/patreon/strengthtest.js:L32` |
| `bet` | `lottery` | `src/commands/commandList/gamble/lottery.js:L13` |
| `bh` | `beehive` | `src/commands/commandList/social/beehive.js:L16` |
| `birthstone` | `birthstone` | `src/commands/commandList/patreon/birthstone.js:L97` |
| `bite` | `bite` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `bj` | `blackjack` | `src/commands/commandList/gamble/blackjack.js:L20` |
| `blackjack` | `blackjack` | `src/commands/commandList/gamble/blackjack.js:L20` |
| `blinkbear` | `blinkbear` | `src/commands/commandList/patreon/collectible.js:L258` |
| `blush` | `blush` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `bnice` | `compliment` | `src/commands/commandList/patreon/compliment.js:L16` |
| `boba` | `boba` | `src/commands/commandList/patreon/boba.js:L26` |
| `bomk` | `bonk` | `src/commands/commandList/patreon/bonk.js:L24` |
| `bonk` | `bonk` | `src/commands/commandList/patreon/bonk.js:L24` |
| `booger` | `booger` | `src/commands/commandList/patreon/collectible.js:L258` |
| `boop` | `boop` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `bouquet` | `rose` | `src/commands/commandList/patreon/rose.js:L17` |
| `broadcasteval` | `broadcasteval` | `src/commands/commandList/admin/broadcastEval.js:L11` |
| `bs` | `battlesetting` | `src/commands/commandList/battle/battleSetting.js:L13` |
| `bsn` | `birthstone` | `src/commands/commandList/patreon/birthstone.js:L97` |
| `bstone` | `birthstone` | `src/commands/commandList/patreon/birthstone.js:L97` |
| `btf` | `butterfly` | `src/commands/commandList/patreon/butterfly.js:L16` |
| `bully` | `bully` | `src/commands/commandList/patreon/bully.js:L29` |
| `bunny` | `bunny` | `src/commands/commandList/patreon/bunny.js:L16` |
| `butcher` | `sacrifice` | `src/commands/commandList/zoo/sacrifice.js:L13` |
| `butterfly` | `butterfly` | `src/commands/commandList/patreon/butterfly.js:L16` |
| `buy` | `buy` | `src/commands/commandList/shop/buy.js:L15` |
| `cake` | `cake` | `src/commands/commandList/patreon/cake.js:L17` |
| `cal` | `calcifer` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `calc` | `math` | `src/commands/commandList/utils/math.js:L16` |
| `calcifer` | `calcifer` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `calcifer` | `calcifer` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `calculate` | `math` | `src/commands/commandList/utils/math.js:L16` |
| `candycane` | `candycane` | `src/commands/commandList/patreon/candycane.js:L16` |
| `captcha` | `captcha` | `src/commands/commandList/admin/captcha.js:L18` |
| `carlspider` | `carlspider` | `src/commands/commandList/patreon/collectible.js:L258` |
| `cash` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `catch` | `hunt` | `src/commands/commandList/zoo/catch.js:L21` |
| `catto` | `shifu` | `src/commands/commandList/patreon/catto.js:L51` |
| `censor` | `censor` | `src/commands/commandList/utils/censor.js:L11` |
| `cf` | `coinflip` | `src/commands/commandList/gamble/coinflip.js:L19` |
| `cg` | `cg` | `src/commands/commandList/admin/creategiveaway.js:L11` |
| `changelog` | `announce` | `src/commands/commandList/utils/announcement.js:L11` |
| `checklist` | `checklist` | `src/commands/commandList/utils/checklist.js:L17` |
| `chicken` | `chicken` | `src/commands/commandList/patreon/chicken.js:L16` |
| `choose` | `choose` | `src/commands/commandList/patreon/choose.js:L21` |
| `chu` | `pikachu` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `cinta` | `dayang3` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `cl` | `checklist` | `src/commands/commandList/utils/checklist.js:L17` |
| `claim` | `claim` | `src/commands/commandList/economy/claim.js:L13` |
| `cloud` | `cloud` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `clover` | `clover` | `src/commands/commandList/patreon/collectible.js:L258` |
| `coffee` | `coffee` | `src/commands/commandList/patreon/coffee.js:L15` |
| `coin` | `coinflip` | `src/commands/commandList/gamble/coinflip.js:L19` |
| `coinflip` | `coinflip` | `src/commands/commandList/gamble/coinflip.js:L19` |
| `color` | `color` | `src/commands/commandList/utils/color.js:L18` |
| `colour` | `color` | `src/commands/commandList/utils/color.js:L18` |
| `combine` | `ship` | `src/commands/commandList/social/ship.js:L13` |
| `communism` | `communism` | `src/commands/commandList/memegen/communism.js:L13` |
| `communismcat` | `communism` | `src/commands/commandList/memegen/communism.js:L13` |
| `compensation` | `claim` | `src/commands/commandList/economy/claim.js:L13` |
| `compliment` | `compliment` | `src/commands/commandList/patreon/compliment.js:L16` |
| `cookie` | `cookie` | `src/commands/commandList/social/cookie.js:L14` |
| `corgi` | `corgi` | `src/commands/commandList/patreon/collectible.js:L258` |
| `coronavirus` | `covid` | `src/commands/commandList/utils/covid.js:L16` |
| `covid` | `covid` | `src/commands/commandList/utils/covid.js:L16` |
| `covid19` | `covid` | `src/commands/commandList/utils/covid.js:L16` |
| `cowoncy` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `cpc` | `cupachicake` | `src/commands/commandList/patreon/cupachicake.js:L15` |
| `crate` | `crate` | `src/commands/commandList/battle/crate.js:L16` |
| `creategiveaway` | `cg` | `src/commands/commandList/admin/creategiveaway.js:L11` |
| `credit` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `crossfox` | `crossfox` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `crossfox` | `crossfox` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `crown` | `crown` | `src/commands/commandList/patreon/crown.js:L15` |
| `cry` | `cry` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `cuddle` | `cuddle` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `cupachicake` | `cupachicake` | `src/commands/commandList/patreon/cupachicake.js:L15` |
| `curly` | `curly` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `currency` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `curse` | `pray` | `src/commands/commandList/social/pray.js:L30` |
| `custompet` | `custompet` | `src/commands/commandList/admin/customPet.js:L47` |
| `cv` | `covid` | `src/commands/commandList/utils/covid.js:L16` |
| `d` | `owodex` | `src/commands/commandList/zoo/owodex.js:L11` |
| `d20` | `roll` | `src/commands/commandList/patreon/dice.js:L28` |
| `daily` | `daily` | `src/commands/commandList/economy/daily.js:L24` |
| `dance` | `dance` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `darwinsfox` | `darwinsfox` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `dayang` | `dayang3` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `dayang3` | `dayang3` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `db` | `db` | `src/commands/commandList/battle/db.js:L11` |
| `death` | `death` | `src/commands/commandList/patreon/death.js:L15` |
| `decide` | `choose` | `src/commands/commandList/patreon/choose.js:L21` |
| `declinebattle` | `db` | `src/commands/commandList/battle/db.js:L11` |
| `declinemarriage` | `declinemarriage` | `src/commands/commandList/social/declineMarriage.js:L13` |
| `define` | `define` | `src/commands/commandList/social/define.js:L15` |
| `deleteuser` | `deleteuser` | `src/commands/commandList/admin/deleteUser.js:L11` |
| `deredere` | `deredere` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `des` | `des` | `src/commands/commandList/patreon/collectible.js:L258` |
| `desc` | `describe` | `src/commands/commandList/shop/describe.js:L17` |
| `describe` | `describe` | `src/commands/commandList/shop/describe.js:L17` |
| `destiny` | `dtn` | `src/commands/commandList/patreon/destiny.js:L36` |
| `devil` | `devil` | `src/commands/commandList/patreon/devil.js:L27` |
| `dex` | `owodex` | `src/commands/commandList/zoo/owodex.js:L11` |
| `dg-hug` | `dg-hug` | `src/commands/commandList/patreon/collectible.js:L258` |
| `dgn` | `dragon` | `src/commands/commandList/patreon/dragon.js:L16` |
| `dhole` | `dhole` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `disable` | `disable` | `src/commands/commandList/utils/disable.js:L13` |
| `disablecaptcha` | `disablecaptcha` | `src/commands/commandList/admin/disableCaptcha.js:L11` |
| `discordplays` | `discordplays` | `src/commands/commandList/social/discordplays.js:L13` |
| `dish` | `dish` | `src/commands/commandList/patreon/dish.js:L14` |
| `dismantle` | `weaponshard` | `src/commands/commandList/battle/weaponshards.js:L32` |
| `distorted` | `distorted` | `src/commands/commandList/utils/distored.js:L21` |
| `distracted` | `distractedbf` | `src/commands/commandList/memegen/distracted.js:L13` |
| `distractedbf` | `distractedbf` | `src/commands/commandList/memegen/distracted.js:L13` |
| `distributecowoncy` | `getpatreons` | `src/commands/commandList/admin/getPatreonRewards.js:L22` |
| `divorce` | `divorce` | `src/commands/commandList/social/divorce.js:L23` |
| `dm` | `declinemarriage` | `src/commands/commandList/social/declineMarriage.js:L13` |
| `doggo` | `corgi` | `src/commands/commandList/patreon/collectible.js:L258` |
| `doll` | `doll` | `src/commands/commandList/patreon/collectible.js:L258` |
| `donate` | `patreon` | `src/commands/commandList/utils/patreon.js:L15` |
| `donut` | `donut` | `src/commands/commandList/patreon/donut.js:L16` |
| `dragon` | `dragon` | `src/commands/commandList/patreon/dragon.js:L16` |
| `drake` | `drake` | `src/commands/commandList/memegen/drake.js:L13` |
| `drop` | `drop` | `src/commands/commandList/gamble/drop.js:L14` |
| `dt` | `distorted` | `src/commands/commandList/utils/distored.js:L21` |
| `dtn` | `dtn` | `src/commands/commandList/patreon/destiny.js:L36` |
| `duwasvivu` | `duwasvivu` | `src/commands/commandList/patreon/duwasvivu.js:L11` |
| `dvl` | `devil` | `src/commands/commandList/patreon/devil.js:L27` |
| `echo` | `echo` | `src/commands/commandList/admin/echo.js:L11` |
| `egg` | `egg` | `src/commands/commandList/patreon/collectible.js:L258` |
| `eightball` | `eightball` | `src/commands/commandList/social/eightball.js:L80` |
| `eject` | `eject` | `src/commands/commandList/memegen/eject.js:L15` |
| `emergency` | `emergency` | `src/commands/commandList/memegen/emergency.js:L16` |
| `emergencymeeting` | `emergency` | `src/commands/commandList/memegen/emergency.js:L16` |
| `emoji` | `emoji` | `src/commands/commandList/social/emoji.js:L14` |
| `emulator` | `discordplays` | `src/commands/commandList/social/discordplays.js:L13` |
| `enable` | `enable` | `src/commands/commandList/utils/enable.js:L14` |
| `enablecaptcha` | `disablecaptcha` | `src/commands/commandList/admin/disableCaptcha.js:L11` |
| `enlarge` | `emoji` | `src/commands/commandList/social/emoji.js:L14` |
| `equip` | `equip` | `src/commands/commandList/shop/equip.js:L18` |
| `essence` | `sacrifice` | `src/commands/commandList/zoo/sacrifice.js:L13` |
| `eval` | `eval` | `src/commands/commandList/admin/eval.js:L11` |
| `ewolf` | `ewolf` | `src/commands/commandList/patreon/collectible.js:L258` |
| `fate` | `fate` | `src/commands/commandList/patreon/fate.js:L22` |
| `fear` | `fear` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `fight` | `battle` | `src/commands/commandList/battle/battle.js:L14` |
| `flame` | `flame` | `src/commands/commandList/patreon/collectible.js:L258` |
| `flip` | `coinflip` | `src/commands/commandList/gamble/coinflip.js:L19` |
| `flm` | `flame` | `src/commands/commandList/patreon/collectible.js:L258` |
| `friend` | `friend` | `src/commands/commandList/patreon/collectible.js:L258` |
| `frogegg` | `frogegg` | `src/commands/commandList/patreon/frogEgg.js:L17` |
| `fuck` | `fuck` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `galikat` | `galikat` | `src/commands/commandList/patreon/collectible.js:L258` |
| `gauntlet` | `gauntlet` | `src/commands/commandList/patreon/gauntlet.js:L18` |
| `gcpt` | `givecustompetticket` | `src/commands/commandList/admin/giveCustomPetTicket.js:L11` |
| `genie` | `genie` | `src/commands/commandList/patreon/genie.js:L26` |
| `getpatreons` | `getpatreons` | `src/commands/commandList/admin/getPatreonRewards.js:L22` |
| `ggt` | `givegiveawayticket` | `src/commands/commandList/admin/giveGiveawayTicket.js:L11` |
| `ghost` | `ghost` | `src/commands/commandList/patreon/collectible.js:L258` |
| `gif` | `gif` | `src/commands/commandList/emotes/images.js:L13` |
| `gift` | `trade` | `src/commands/commandList/shop/trade.js:L17` |
| `ginseng` | `ginseng` | `src/commands/commandList/patreon/collectible.js:L258` |
| `give` | `give` | `src/commands/commandList/economy/give.js:L20` |
| `giveall` | `giveall` | `src/commands/commandList/admin/giveall.js:L11` |
| `givecustompetticket` | `givecustompetticket` | `src/commands/commandList/admin/giveCustomPetTicket.js:L11` |
| `givegiveawayticket` | `givegiveawayticket` | `src/commands/commandList/admin/giveGiveawayTicket.js:L11` |
| `giveperkticket` | `giveperkticket` | `src/commands/commandList/admin/givePerkTicket.js:L11` |
| `giveticket` | `giveperkticket` | `src/commands/commandList/admin/givePerkTicket.js:L11` |
| `goldenegg` | `goldenegg` | `src/commands/commandList/patreon/goldenegg.js:L15` |
| `greet` | `greet` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `grim` | `grim` | `src/commands/commandList/patreon/grim.js:L11` |
| `grin` | `grin` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `grizzly` | `grizzly` | `src/commands/commandList/patreon/collectible.js:L258` |
| `guild` | `my` | `src/commands/commandList/ranking/me.js:L22` |
| `guildlink` | `guildlink` | `src/commands/commandList/utils/guildlink.js:L11` |
| `guillotine` | `guillotine` | `src/commands/commandList/patreon/guillotine.js:L17` |
| `h` | `hunt` | `src/commands/commandList/zoo/catch.js:L21` |
| `handholding` | `handholding` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `happy` | `happy` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `hauntedhouse` | `hauntedhouse` | `src/commands/commandList/patreon/hauntedhouse.js:L14` |
| `hb` | `autohunt` | `src/commands/commandList/zoo/autohunt.js:L22` |
| `headpat` | `headpat` | `src/commands/commandList/memegen/headpat.js:L14` |
| `heart` | `smokeheart` | `src/commands/commandList/patreon/collectible.js:L258` |
| `help` | `help` | `src/commands/commandList/utils/help.js:L22` |
| `highfive` | `highfive` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `hive` | `beehive` | `src/commands/commandList/social/beehive.js:L16` |
| `hold` | `hold` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `honey` | `bee` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `hongbao` | `redenvelope` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `hug` | `hug` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `hunt` | `hunt` | `src/commands/commandList/zoo/catch.js:L21` |
| `huntbot` | `autohunt` | `src/commands/commandList/zoo/autohunt.js:L22` |
| `husband` | `propose` | `src/commands/commandList/social/marry.js:L45` |
| `icecream` | `icecream` | `src/commands/commandList/patreon/icecream.js:L24` |
| `ify` | `owo` | `src/commands/commandList/social/owoify.js:L14` |
| `indonesia` | `dayang3` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `info` | `stats` | `src/commands/commandList/utils/stats.js:L12` |
| `inv` | `inventory` | `src/commands/commandList/shop/inventory.js:L21` |
| `inventory` | `inventory` | `src/commands/commandList/shop/inventory.js:L21` |
| `invite` | `invite` | `src/commands/commandList/utils/invite.js:L11` |
| `isthisa` | `isthisa` | `src/commands/commandList/memegen/isthisa.js:L15` |
| `java` | `coffee` | `src/commands/commandList/patreon/coffee.js:L15` |
| `jester` | `chicken` | `src/commands/commandList/patreon/chicken.js:L16` |
| `jumbo` | `emoji` | `src/commands/commandList/social/emoji.js:L14` |
| `kasih` | `des` | `src/commands/commandList/patreon/collectible.js:L258` |
| `kfire` | `kfire` | `src/commands/commandList/patreon/collectible.js:L258` |
| `kill` | `kill` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `king` | `king` | `src/commands/commandList/patreon/king.js:L27` |
| `kiss` | `kiss` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `kitty` | `kitty` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `koi` | `koi` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `koi` | `koi` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `larry` | `larry` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `latte` | `latte` | `src/commands/commandList/patreon/latte.js:L26` |
| `lb` | `lootbox` | `src/commands/commandList/zoo/lootbox.js:L20` |
| `lc` | `liftcommand` | `src/commands/commandList/admin/liftCommand.js:L13` |
| `lemon` | `lemon` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `lemonade` | `lemon` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `level` | `level` | `src/commands/commandList/social/level.js:L14` |
| `levels` | `level` | `src/commands/commandList/social/level.js:L14` |
| `lewd` | `lewd` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `lick` | `lick` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `life` | `life` | `src/commands/commandList/patreon/life.js:L15` |
| `lift` | `lift` | `src/commands/commandList/admin/lift.js:L11` |
| `liftcommand` | `liftcommand` | `src/commands/commandList/admin/liftCommand.js:L13` |
| `lilbee` | `lilbee` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `lilbee` | `lilbee` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `link` | `invite` | `src/commands/commandList/utils/invite.js:L11` |
| `listlang` | `translate` | `src/commands/commandList/social/translate.js:L13` |
| `lmn` | `lemon` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `ln` | `lovenote` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `lollipop` | `lollipop` | `src/commands/commandList/patreon/lollipop.js:L16` |
| `lootbox` | `lootbox` | `src/commands/commandList/zoo/lootbox.js:L20` |
| `lottery` | `lottery` | `src/commands/commandList/gamble/lottery.js:L13` |
| `lotto` | `lottery` | `src/commands/commandList/gamble/lottery.js:L13` |
| `lotus` | `koi` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `love` | `love` | `src/commands/commandList/patreon/love.js:L15` |
| `lovenote` | `lovenote` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `lovey` | `luv` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `luv` | `luv` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `luv` | `luv` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `lvl` | `level` | `src/commands/commandList/social/level.js:L14` |
| `lxv` | `lxv` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `magic` | `magic` | `src/commands/commandList/patreon/magic.js:L27` |
| `magoo` | `magoo` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `market` | `shop` | `src/commands/commandList/shop/shop.js:L26` |
| `marriage` | `propose` | `src/commands/commandList/social/marry.js:L45` |
| `marry` | `propose` | `src/commands/commandList/social/marry.js:L45` |
| `martini` | `martini` | `src/commands/commandList/patreon/collectible.js:L258` |
| `math` | `math` | `src/commands/commandList/utils/math.js:L16` |
| `me` | `my` | `src/commands/commandList/ranking/me.js:L22` |
| `melanisticfox` | `crossfox` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `meshi` | `meshi` | `src/commands/commandList/patreon/meshi.js:L15` |
| `milk` | `milk` | `src/commands/commandList/patreon/milk.js:L16` |
| `mochi` | `mochi` | `src/commands/commandList/patreon/mochi.js:L28` |
| `moe` | `moe` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `money` | `cowoncy` | `src/commands/commandList/economy/cowoncy.js:L12` |
| `moon` | `moon` | `src/commands/commandList/patreon/moon.js:L28` |
| `msc` | `music` | `src/commands/commandList/patreon/collectible.js:L258` |
| `msgusers` | `msgusers` | `src/commands/commandList/admin/msgUsers.js:L11` |
| `music` | `music` | `src/commands/commandList/patreon/collectible.js:L258` |
| `my` | `my` | `src/commands/commandList/ranking/me.js:L22` |
| `nier` | `nier` | `src/commands/commandList/patreon/nier.js:L15` |
| `nom` | `nom` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `nommy` | `fear` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `obw` | `obw` | `src/commands/commandList/patreon/obw.js:L15` |
| `obwspecial` | `obwspecial` | `src/commands/commandList/patreon/collectible.js:L258` |
| `od` | `owodex` | `src/commands/commandList/zoo/owodex.js:L11` |
| `owo` | `owo` | `src/commands/commandList/social/owoify.js:L14` |
| `owodex` | `owodex` | `src/commands/commandList/zoo/owodex.js:L11` |
| `owoify` | `owo` | `src/commands/commandList/social/owoify.js:L14` |
| `painted-dog` | `painteddog` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `painteddog` | `painteddog` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `pancakes` | `pancakes` | `src/commands/commandList/patreon/collectible.js:L258` |
| `panda` | `panda` | `src/commands/commandList/patreon/collectible.js:L258` |
| `pat` | `pat` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `patreon` | `patreon` | `src/commands/commandList/utils/patreon.js:L15` |
| `pats` | `pats` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `pausebot` | `pausebot` | `src/commands/commandList/admin/pauseBot.js:L11` |
| `penguin` | `penguin` | `src/commands/commandList/patreon/collectible.js:L258` |
| `pet` | `pets` | `src/commands/commandList/battle/pet.js:L14` |
| `pets` | `pets` | `src/commands/commandList/battle/pet.js:L14` |
| `pgn` | `penguin` | `src/commands/commandList/patreon/collectible.js:L258` |
| `pic` | `gif` | `src/commands/commandList/emotes/images.js:L13` |
| `pick` | `choose` | `src/commands/commandList/patreon/choose.js:L21` |
| `pickup` | `drop` | `src/commands/commandList/gamble/drop.js:L14` |
| `pika` | `pika` | `src/commands/commandList/patreon/pika.js:L11` |
| `pikachu` | `pikachu` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `pikachu` | `pikachu` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `pikapika` | `pika` | `src/commands/commandList/patreon/pika.js:L11` |
| `piku` | `piku` | `src/commands/commandList/patreon/piku.js:L17` |
| `ping` | `ping` | `src/commands/commandList/utils/ping.js:L13` |
| `pizza` | `pizza` | `src/commands/commandList/patreon/pizza.js:L15` |
| `planet` | `planet` | `src/commands/commandList/patreon/planet.js:L75` |
| `points` | `points` | `src/commands/commandList/points.js:L11` |
| `poison` | `poison` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `poke` | `poke` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `pong` | `ping` | `src/commands/commandList/utils/ping.js:L13` |
| `pout` | `pout` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `poutine` | `poutine` | `src/commands/commandList/patreon/poutine.js:L24` |
| `pray` | `pray` | `src/commands/commandList/social/pray.js:L30` |
| `prayfrom` | `prayfrom` | `src/commands/commandList/admin/prayfrom.js:L22` |
| `prayto` | `prayto` | `src/commands/commandList/admin/prayto.js:L22` |
| `prefix` | `prefix` | `src/commands/commandList/utils/prefix.js:L29` |
| `profile` | `profile` | `src/commands/commandList/social/profile.js:L13` |
| `propose` | `propose` | `src/commands/commandList/social/marry.js:L45` |
| `punch` | `punch` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `pup` | `puppy` | `src/commands/commandList/patreon/puppy.js:L14` |
| `puppy` | `puppy` | `src/commands/commandList/patreon/puppy.js:L14` |
| `q` | `quest` | `src/commands/commandList/economy/quest.js:L20` |
| `queen` | `queen` | `src/commands/commandList/patreon/queen.js:L27` |
| `quest` | `quest` | `src/commands/commandList/economy/quest.js:L20` |
| `ra` | `refreshanimals` | `src/commands/commandList/admin/refreshAnimals.js:L11` |
| `rain` | `rainbow` | `src/commands/commandList/patreon/rain.js:L42` |
| `rainbow` | `rainbow` | `src/commands/commandList/patreon/rain.js:L42` |
| `raindrop` | `rainbow` | `src/commands/commandList/patreon/rain.js:L42` |
| `randcolor` | `color` | `src/commands/commandList/utils/color.js:L18` |
| `randcolour` | `color` | `src/commands/commandList/utils/color.js:L18` |
| `rank` | `top` | `src/commands/commandList/ranking/top.js:L22` |
| `ranking` | `top` | `src/commands/commandList/ranking/top.js:L22` |
| `redenvelope` | `redenvelope` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `redwolf` | `redwolf` | `src/commands/commandList/patreon/collectible.js:L258` |
| `refreshanimals` | `refreshanimals` | `src/commands/commandList/admin/refreshAnimals.js:L11` |
| `regret` | `regret` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `removeoptout` | `removeoptout` | `src/commands/commandList/admin/removeOptOut.js:L11` |
| `removestrike` | `removestrike` | `src/commands/commandList/admin/removeStrike.js:L11` |
| `rename` | `rename` | `src/commands/commandList/battle/rename.js:L11` |
| `rep` | `cookie` | `src/commands/commandList/social/cookie.js:L14` |
| `reply` | `reply` | `src/commands/commandList/admin/reply.js:L11` |
| `resetbot` | `resetbot` | `src/commands/commandList/admin/resetbot.js:L11` |
| `resetcowoncy` | `resetcowoncy` | `src/commands/commandList/admin/resetCowoncy.js:L11` |
| `resetowo` | `resetowo` | `src/commands/commandList/admin/resetOwo.js:L11` |
| `restartbot` | `resetbot` | `src/commands/commandList/admin/resetbot.js:L11` |
| `reward` | `claim` | `src/commands/commandList/economy/claim.js:L13` |
| `roll` | `roll` | `src/commands/commandList/patreon/dice.js:L28` |
| `roo` | `removeoptout` | `src/commands/commandList/admin/removeOptOut.js:L11` |
| `rose` | `rose` | `src/commands/commandList/patreon/rose.js:L17` |
| `rule` | `rule` | `src/commands/commandList/utils/rules.js:L20` |
| `rules` | `rule` | `src/commands/commandList/utils/rules.js:L20` |
| `rum` | `rum` | `src/commands/commandList/patreon/rum.js:L14` |
| `run` | `run` | `src/commands/commandList/patreon/run.js:L14` |
| `s` | `slots` | `src/commands/commandList/gamble/slots.js:L24` |
| `sac` | `sacrifice` | `src/commands/commandList/zoo/sacrifice.js:L13` |
| `sacrifice` | `sacrifice` | `src/commands/commandList/zoo/sacrifice.js:L13` |
| `sakura` | `sakura` | `src/commands/commandList/patreon/sakura.js:L15` |
| `sammy` | `sammy` | `src/commands/commandList/patreon/collectible.js:L258` |
| `saturn` | `saturn` | `src/commands/commandList/patreon/collectible.js:L258` |
| `sayang` | `dg-hug` | `src/commands/commandList/patreon/collectible.js:L258` |
| `sc` | `sacrifice` | `src/commands/commandList/zoo/sacrifice.js:L13` |
| `schicken` | `spongebobchicken` | `src/commands/commandList/memegen/spongebobchicken.js:L14` |
| `scoff` | `scoff` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `sell` | `sell` | `src/commands/commandList/zoo/sell.js:L14` |
| `send` | `give` | `src/commands/commandList/economy/give.js:L20` |
| `sendverif` | `sendverif` | `src/commands/commandList/admin/sendverif.js:L13` |
| `setcaptcha` | `disablecaptcha` | `src/commands/commandList/admin/disableCaptcha.js:L11` |
| `setstrike` | `removestrike` | `src/commands/commandList/admin/removeStrike.js:L11` |
| `setteam` | `teams` | `src/commands/commandList/battle/teams.js:L15` |
| `sex` | `sex` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `shard` | `shards` | `src/commands/commandList/utils/shard.js:L17` |
| `shards` | `shards` | `src/commands/commandList/utils/shard.js:L17` |
| `sharingan` | `sharingan` | `src/commands/commandList/patreon/sharingan.js:L14` |
| `shemp` | `shemp` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `shifu` | `shifu` | `src/commands/commandList/patreon/catto.js:L51` |
| `ship` | `ship` | `src/commands/commandList/social/ship.js:L13` |
| `shootingstar` | `shootingstar` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `shootingstar` | `shootingstar` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `shop` | `shop` | `src/commands/commandList/shop/shop.js:L26` |
| `shrug` | `shrug` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `slap` | `slap` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `slapcar` | `slapcar` | `src/commands/commandList/memegen/slapcar.js:L16` |
| `slaproof` | `slapcar` | `src/commands/commandList/memegen/slapcar.js:L16` |
| `sleepy` | `sleepy` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `slime` | `slime` | `src/commands/commandList/patreon/slime.js:L16` |
| `slot` | `slots` | `src/commands/commandList/gamble/slots.js:L24` |
| `slots` | `slots` | `src/commands/commandList/gamble/slots.js:L24` |
| `smile` | `smile` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `smokeheart` | `smokeheart` | `src/commands/commandList/patreon/collectible.js:L258` |
| `smug` | `smug` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `snake` | `snake` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `snowball` | `snowball` | `src/commands/commandList/patreon/snowball.js:L15` |
| `snuggle` | `snuggle` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `sonic` | `sonic` | `src/commands/commandList/patreon/collectible.js:L258` |
| `soot` | `sootsprite` | `src/commands/commandList/patreon/collectible.js:L258` |
| `sootgremlin` | `sootsprite` | `src/commands/commandList/patreon/collectible.js:L258` |
| `sootsprite` | `sootsprite` | `src/commands/commandList/patreon/collectible.js:L258` |
| `spider` | `spider` | `src/commands/commandList/patreon/collectible.js:L258` |
| `spongebobchicken` | `spongebobchicken` | `src/commands/commandList/memegen/spongebobchicken.js:L14` |
| `squad` | `team` | `src/commands/commandList/battle/team.js:L15` |
| `squads` | `teams` | `src/commands/commandList/battle/teams.js:L15` |
| `ss` | `shootingstar` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `star` | `star` | `src/commands/commandList/patreon/collectible.js:L258` |
| `stare` | `stare` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `stat` | `stats` | `src/commands/commandList/utils/stats.js:L12` |
| `stats` | `stats` | `src/commands/commandList/utils/stats.js:L12` |
| `stitch` | `stitch` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `strengthtest` | `bell` | `src/commands/commandList/patreon/strengthtest.js:L32` |
| `suggest` | `suggest` | `src/commands/commandList/utils/suggest.js:L20` |
| `sun` | `sun` | `src/commands/commandList/patreon/sun.js:L28` |
| `sunflower` | `sunflower` | `src/commands/commandList/patreon/sunflower.js:L15` |
| `support` | `patreon` | `src/commands/commandList/utils/patreon.js:L15` |
| `supporter` | `patreon` | `src/commands/commandList/utils/patreon.js:L15` |
| `survey` | `survey` | `src/commands/commandList/utils/survey.js:L13` |
| `susuwatari` | `sootsprite` | `src/commands/commandList/patreon/collectible.js:L258` |
| `taco` | `taco` | `src/commands/commandList/patreon/taco.js:L16` |
| `tarot` | `tarot` | `src/commands/commandList/patreon/tarot.js:L74` |
| `task` | `checklist` | `src/commands/commandList/utils/checklist.js:L17` |
| `tasks` | `checklist` | `src/commands/commandList/utils/checklist.js:L17` |
| `td` | `truthordare` | `src/commands/commandList/patreon/truthordare.js:L96` |
| `te` | `testevent` | `src/commands/commandList/admin/testEvent.js:L11` |
| `team` | `team` | `src/commands/commandList/battle/team.js:L15` |
| `teams` | `teams` | `src/commands/commandList/battle/teams.js:L15` |
| `teddy` | `teddy` | `src/commands/commandList/patreon/collectible.js:L258` |
| `teehee` | `teehee` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `tequila` | `tequila` | `src/commands/commandList/patreon/tequila.js:L35` |
| `testevent` | `testevent` | `src/commands/commandList/admin/testEvent.js:L11` |
| `thinking` | `thinking` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `thonking` | `thonking` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `thumbs` | `thumbs` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `thumbsup` | `thumbsup` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `tickle` | `tickle` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `tl` | `translate` | `src/commands/commandList/social/translate.js:L13` |
| `tm` | `team` | `src/commands/commandList/battle/team.js:L15` |
| `top` | `top` | `src/commands/commandList/ranking/top.js:L22` |
| `totoro` | `totoro` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `tr` | `trade` | `src/commands/commandList/shop/trade.js:L17` |
| `trade` | `trade` | `src/commands/commandList/shop/trade.js:L17` |
| `tradeoffer` | `tradeoffer` | `src/commands/commandList/memegen/tradeoffer.js:L13` |
| `transaction` | `transaction` | `src/commands/commandList/admin/transaction.js:L22` |
| `translate` | `translate` | `src/commands/commandList/social/translate.js:L13` |
| `triggered` | `triggered` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `truthordare` | `truthordare` | `src/commands/commandList/patreon/truthordare.js:L96` |
| `turnip` | `turnip` | `src/commands/commandList/patreon/turnip.js:L27` |
| `twitchplays` | `discordplays` | `src/commands/commandList/social/discordplays.js:L13` |
| `ufo` | `shifu` | `src/commands/commandList/patreon/catto.js:L51` |
| `uncensor` | `uncensor` | `src/commands/commandList/utils/uncensor.js:L11` |
| `unicorn` | `unicorn` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `upg` | `upgrade` | `src/commands/commandList/zoo/upgrade.js:L28` |
| `upgrade` | `upgrade` | `src/commands/commandList/zoo/upgrade.js:L28` |
| `use` | `equip` | `src/commands/commandList/shop/equip.js:L18` |
| `user` | `avatar` | `src/commands/commandList/utils/avatar.js:L11` |
| `useteams` | `teams` | `src/commands/commandList/battle/teams.js:L15` |
| `vert` | `vert` | `src/commands/commandList/patreon/collectibleClasses.js:L25` |
| `vote` | `vote` | `src/commands/commandList/utils/vote.js:L26` |
| `w` | `weapon` | `src/commands/commandList/battle/weapon.js:L16` |
| `waddle` | `waddle` | `src/commands/commandList/memegen/waddle.js:L14` |
| `wag` | `wag` | `src/commands/commandList/emotes/self_emote.js:L16` |
| `wallpaper` | `wallpaper` | `src/commands/commandList/social/wallpaper.js:L16` |
| `wallpapers` | `wallpaper` | `src/commands/commandList/social/wallpaper.js:L16` |
| `warn` | `warn` | `src/commands/commandList/admin/warn.js:L11` |
| `water` | `water` | `src/commands/commandList/patreon/water.js:L17` |
| `wave` | `wave` | `src/commands/commandList/emotes/user_emote.js:L16` |
| `wc` | `crate` | `src/commands/commandList/battle/crate.js:L16` |
| `weapon` | `weapon` | `src/commands/commandList/battle/weapon.js:L16` |
| `weaponcrate` | `crate` | `src/commands/commandList/battle/crate.js:L16` |
| `weapons` | `weapon` | `src/commands/commandList/battle/weapon.js:L16` |
| `weaponshard` | `weaponshard` | `src/commands/commandList/battle/weaponshards.js:L32` |
| `weaponshards` | `weaponshard` | `src/commands/commandList/battle/weaponshards.js:L32` |
| `wep` | `weapon` | `src/commands/commandList/battle/weapon.js:L16` |
| `wet` | `rainbow` | `src/commands/commandList/patreon/rain.js:L42` |
| `wife` | `propose` | `src/commands/commandList/social/marry.js:L45` |
| `witch` | `witch` | `src/commands/commandList/patreon/collectible.js:L258` |
| `wolf` | `wolf` | `src/commands/commandList/patreon/collectible.js:L258` |
| `wp` | `wallpaper` | `src/commands/commandList/social/wallpaper.js:L16` |
| `ws` | `weaponshard` | `src/commands/commandList/battle/weaponshards.js:L32` |
| `xp` | `level` | `src/commands/commandList/social/level.js:L14` |
| `yinyang` | `yinyang` | `src/commands/commandList/patreon/yinyang.js:L15` |
| `yy` | `yinyang` | `src/commands/commandList/patreon/yinyang.js:L15` |
| `z` | `zoo` | `src/commands/commandList/zoo/zoo.js:L15` |
| `zk` | `zodiackey` | `src/commands/commandList/patreon/zodiackey.js:L68` |
| `zodiackey` | `zodiackey` | `src/commands/commandList/patreon/zodiackey.js:L68` |
| `zoo` | `zoo` | `src/commands/commandList/zoo/zoo.js:L15` |

## Appendix B — Commands With NO Aliases

- `addannouncement` — `src/commands/commandList/admin/addAnnouncement.js:L11`
- `addbattle` — `src/commands/commandList/admin/addBattle.js:L14`
- `addcookie` — `src/commands/commandList/admin/addCookie.js:L14`
- `addcowoncy` — `src/commands/commandList/admin/addCowoncy.js:L14`
- `adddaily` — `src/commands/commandList/admin/addDaily.js:L14`
- `addgive` — `src/commands/commandList/admin/addGive.js:L14`
- `addhunt` — `src/commands/commandList/admin/addHunt.js:L14`
- `addinventory` — `src/commands/commandList/admin/addInventory.js:L14`
- `addpet` — `src/commands/commandList/admin/addPet.js:L11`
- `addpray` — `src/commands/commandList/admin/addPray.js:L14`
- `addweapon` — `src/commands/commandList/admin/addWeapon.js:L14`
- `addzoo` — `src/commands/commandList/admin/addZoo.js:L14`
- `adminprofile` — `src/commands/commandList/admin/adminProfile.js:L13`
- `ban` — `src/commands/commandList/admin/ban.js:L13`
- `banguildmembers` — `src/commands/commandList/admin/banGuildMembers.js:L11`
- `banstatus` — `src/commands/commandList/admin/banstatus.js:L11`
- `broadcasteval` — `src/commands/commandList/admin/broadcastEval.js:L11`
- `captcha` — `src/commands/commandList/admin/captcha.js:L18`
- `custompet` — `src/commands/commandList/admin/customPet.js:L47`
- `deleteuser` — `src/commands/commandList/admin/deleteUser.js:L11`
- `echo` — `src/commands/commandList/admin/echo.js:L11`
- `eval` — `src/commands/commandList/admin/eval.js:L11`
- `giveall` — `src/commands/commandList/admin/giveall.js:L11`
- `lift` — `src/commands/commandList/admin/lift.js:L11`
- `msgusers` — `src/commands/commandList/admin/msgUsers.js:L11`
- `pausebot` — `src/commands/commandList/admin/pauseBot.js:L11`
- `prayfrom` — `src/commands/commandList/admin/prayfrom.js:L22`
- `prayto` — `src/commands/commandList/admin/prayto.js:L22`
- `reply` — `src/commands/commandList/admin/reply.js:L11`
- `resetcowoncy` — `src/commands/commandList/admin/resetCowoncy.js:L11`
- `resetowo` — `src/commands/commandList/admin/resetOwo.js:L11`
- `sendverif` — `src/commands/commandList/admin/sendverif.js:L13`
- `transaction` — `src/commands/commandList/admin/transaction.js:L22`
- `warn` — `src/commands/commandList/admin/warn.js:L11`
- `rename` — `src/commands/commandList/battle/rename.js:L11`
- `daily` — `src/commands/commandList/economy/daily.js:L24`
- `drake` — `src/commands/commandList/memegen/drake.js:L13`
- `headpat` — `src/commands/commandList/memegen/headpat.js:L14`
- `isthisa` — `src/commands/commandList/memegen/isthisa.js:L15`
- `tradeoffer` — `src/commands/commandList/memegen/tradeoffer.js:L13`
- `waddle` — `src/commands/commandList/memegen/waddle.js:L14`
- `02kiss` — `src/commands/commandList/patreon/02kiss.js:L13`
- `alastor` — `src/commands/commandList/patreon/alastor.js:L22`
- `army` — `src/commands/commandList/patreon/army.js:L19`
- `babyyoda` — `src/commands/commandList/patreon/babyyoda.js:L26`
- `boba` — `src/commands/commandList/patreon/boba.js:L26`
- `bully` — `src/commands/commandList/patreon/bully.js:L29`
- `bunny` — `src/commands/commandList/patreon/bunny.js:L16`
- `cake` — `src/commands/commandList/patreon/cake.js:L17`
- `candycane` — `src/commands/commandList/patreon/candycane.js:L16`
- `crown` — `src/commands/commandList/patreon/crown.js:L15`
- `death` — `src/commands/commandList/patreon/death.js:L15`
- `dish` — `src/commands/commandList/patreon/dish.js:L14`
- `donut` — `src/commands/commandList/patreon/donut.js:L16`
- `duwasvivu` — `src/commands/commandList/patreon/duwasvivu.js:L11`
- `fate` — `src/commands/commandList/patreon/fate.js:L22`
- `frogegg` — `src/commands/commandList/patreon/frogEgg.js:L17`
- `gauntlet` — `src/commands/commandList/patreon/gauntlet.js:L18`
- `genie` — `src/commands/commandList/patreon/genie.js:L26`
- `goldenegg` — `src/commands/commandList/patreon/goldenegg.js:L15`
- `grim` — `src/commands/commandList/patreon/grim.js:L11`
- `guillotine` — `src/commands/commandList/patreon/guillotine.js:L17`
- `hauntedhouse` — `src/commands/commandList/patreon/hauntedhouse.js:L14`
- `icecream` — `src/commands/commandList/patreon/icecream.js:L24`
- `king` — `src/commands/commandList/patreon/king.js:L27`
- `latte` — `src/commands/commandList/patreon/latte.js:L26`
- `life` — `src/commands/commandList/patreon/life.js:L15`
- `lollipop` — `src/commands/commandList/patreon/lollipop.js:L16`
- `love` — `src/commands/commandList/patreon/love.js:L15`
- `magic` — `src/commands/commandList/patreon/magic.js:L27`
- `meshi` — `src/commands/commandList/patreon/meshi.js:L15`
- `milk` — `src/commands/commandList/patreon/milk.js:L16`
- `mochi` — `src/commands/commandList/patreon/mochi.js:L28`
- `moon` — `src/commands/commandList/patreon/moon.js:L28`
- `nier` — `src/commands/commandList/patreon/nier.js:L15`
- `obw` — `src/commands/commandList/patreon/obw.js:L15`
- `piku` — `src/commands/commandList/patreon/piku.js:L17`
- `pizza` — `src/commands/commandList/patreon/pizza.js:L15`
- `planet` — `src/commands/commandList/patreon/planet.js:L75`
- `poutine` — `src/commands/commandList/patreon/poutine.js:L24`
- `queen` — `src/commands/commandList/patreon/queen.js:L27`
- `rum` — `src/commands/commandList/patreon/rum.js:L14`
- `run` — `src/commands/commandList/patreon/run.js:L14`
- `sakura` — `src/commands/commandList/patreon/sakura.js:L15`
- `sharingan` — `src/commands/commandList/patreon/sharingan.js:L14`
- `slime` — `src/commands/commandList/patreon/slime.js:L16`
- `snowball` — `src/commands/commandList/patreon/snowball.js:L15`
- `sun` — `src/commands/commandList/patreon/sun.js:L28`
- `sunflower` — `src/commands/commandList/patreon/sunflower.js:L15`
- `taco` — `src/commands/commandList/patreon/taco.js:L16`
- `tarot` — `src/commands/commandList/patreon/tarot.js:L74`
- `tequila` — `src/commands/commandList/patreon/tequila.js:L35`
- `turnip` — `src/commands/commandList/patreon/turnip.js:L27`
- `water` — `src/commands/commandList/patreon/water.js:L17`
- `points` — `src/commands/commandList/points.js:L11`
- `buy` — `src/commands/commandList/shop/buy.js:L15`
- `define` — `src/commands/commandList/social/define.js:L15`
- `divorce` — `src/commands/commandList/social/divorce.js:L23`
- `profile` — `src/commands/commandList/social/profile.js:L13`
- `censor` — `src/commands/commandList/utils/censor.js:L11`
- `disable` — `src/commands/commandList/utils/disable.js:L13`
- `enable` — `src/commands/commandList/utils/enable.js:L14`
- `guildlink` — `src/commands/commandList/utils/guildlink.js:L11`
- `help` — `src/commands/commandList/utils/help.js:L22`
- `prefix` — `src/commands/commandList/utils/prefix.js:L29`
- `suggest` — `src/commands/commandList/utils/suggest.js:L20`
- `survey` — `src/commands/commandList/utils/survey.js:L13`
- `uncensor` — `src/commands/commandList/utils/uncensor.js:L11`
- `vote` — `src/commands/commandList/utils/vote.js:L26`
- `sell` — `src/commands/commandList/zoo/sell.js:L14`
- `bear` — `src/commands/commandList/patreon/collectible.js:L258`
- `ginseng` — `src/commands/commandList/patreon/collectible.js:L258`
- `grizzly` — `src/commands/commandList/patreon/collectible.js:L258`
- `panda` — `src/commands/commandList/patreon/collectible.js:L258`
- `sonic` — `src/commands/commandList/patreon/collectible.js:L258`
- `teddy` — `src/commands/commandList/patreon/collectible.js:L258`
- `carlspider` — `src/commands/commandList/patreon/collectible.js:L258`
- `star` — `src/commands/commandList/patreon/collectible.js:L258`
- `saturn` — `src/commands/commandList/patreon/collectible.js:L258`
- `spider` — `src/commands/commandList/patreon/collectible.js:L258`
- `doll` — `src/commands/commandList/patreon/collectible.js:L258`
- `martini` — `src/commands/commandList/patreon/collectible.js:L258`
- `wolf` — `src/commands/commandList/patreon/collectible.js:L258`
- `pancakes` — `src/commands/commandList/patreon/collectible.js:L258`
- `booger` — `src/commands/commandList/patreon/collectible.js:L258`
- `galikat` — `src/commands/commandList/patreon/collectible.js:L258`
- `kfire` — `src/commands/commandList/patreon/collectible.js:L258`
- `egg` — `src/commands/commandList/patreon/collectible.js:L258`
- `sammy` — `src/commands/commandList/patreon/collectible.js:L258`
- `ewolf` — `src/commands/commandList/patreon/collectible.js:L258`
- `friend` — `src/commands/commandList/patreon/collectible.js:L258`
- `ghost` — `src/commands/commandList/patreon/collectible.js:L258`
- `witch` — `src/commands/commandList/patreon/collectible.js:L258`
- `bat` — `src/commands/commandList/patreon/collectible.js:L258`
- `clover` — `src/commands/commandList/patreon/collectible.js:L258`
- `blinkbear` — `src/commands/commandList/patreon/collectible.js:L258`
- `redwolf` — `src/commands/commandList/patreon/collectible.js:L258`
- `cloud` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `curly` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `darwinsfox` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `dhole` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `kitty` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `larry` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `lxv` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `magoo` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `moe` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `poison` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `regret` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `shemp` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `snake` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `stitch` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `totoro` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `unicorn` — `src/commands/commandList/patreon/collectibleClasses.js:L25`
- `vert` — `src/commands/commandList/patreon/collectibleClasses.js:L25`

## Appendix C — Orphaned Definitions (defined but not loaded)

The loader at `src/commands/command.js:239` walks every module exported from `src/commands/commandList/` and loads every `CommandInterface` it finds (either as a direct export or inside an exported array).  Every command file enumerated in this document uses one of those two patterns, so no orphaned definitions were found.

None found.

## Appendix D — Duplicate Alias Conflicts

*None found.*  Every alias resolves to a unique command.

## Appendix E — Ambiguity & Dynamic Alias Notes

The following commands have aliases or definitions that are not literal JavaScript arrays in a single file — their aliases are derived statically at module-load time from other source-of-truth files:

- **`self_emote` / `user_emote`** (`src/commands/commandList/emotes/self_emote.js`, `.../user_emote.js`):  aliases come from the keys of `sEmote` / `uEmote` in `src/data/emotes.json`.  `distinctAlias: true`, so every alias is its own registered command name.
- **`collectible.js`** (`src/commands/commandList/patreon/collectible.js`):  iterates over entries in `src/commands/commandList/patreon/utils/collectibles.json` and creates one `CommandInterface` per entry with alias `[dataName, ...alias]`.
- **`collectibleClasses.js`** (`src/commands/commandList/patreon/collectibleClasses.js`):  loads every file in `src/commands/commandList/patreon/collectibles/` (except `CollectibleInterface.js`) via `require-dir` and creates one `CommandInterface` per class with alias `[this.key, ...this.alias]` (see each file under that directory).

