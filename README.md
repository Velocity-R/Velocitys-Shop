# Velocity's Shop

## Description

So what actually is this? It's just my dream-project economy plugin that has a couple of pretty cool features (at least in my opinion):
- Sending money to other players
- Auction House for selling custom items [WIP]
- Fluctuating prices influenced by recent buying/selling habits based on the whole server (See more below) [WIP]
- And more to come

## Roadmap

```mermaid
flowchart LR
    %% Phase# --> Phase#[Major Update: ] P#_Sub#[Minor Update: ]

    Start[Initial Shop Release] --> Phase1[Major Update: Fluctuating Pricing]
    Phase1 --> Phase2[Major Update: Auction House]
    Phase2 --> Phase3[Major Update: TBD]
    Phase3 --> End[Major Update: TBD]
```

## Commands

| Command | Description |
| --- | --- |
| ```/shop``` | Opens the main shop page |
| ```/shop [page]``` | Opens a specific shop page |
| ```/bal``` | Shows your available balance |
| ```/baltop``` | Shows the balances of all players |
| ```/buy [itemname] [amount]``` | Allows you to buy items without opening the shop |
| ```/sell``` | Sells the item that's in your hand |
| ```/sellallhand``` | Sells all the item(s) that are in your hand & inventory |
| ```/sellall [itemname]``` | Sells all the item(s) that match the one you specified |
| ```/ah``` | [**In-development**] Opens the auction house |
| ```/send [playername] [amount]``` | Lets you send any amount to the specified player |

## Fluctuating Prices

As mentioned in the description, this plugin has a very cool pricing system. To be put in simple terms, supply and demand. In a more in-depth explanation the plugin has a section that only listens for the ```/buy``` and ```/sell``` commands and whenever someone buys something from the shop gui. Then after logging the recent activity, it then compares that to previous data to determine how much he price should vary by.
