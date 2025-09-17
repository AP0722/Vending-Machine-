# Overview
The Vending Machine plugin allows players to create and manage functional vending machines in Minecraft.
Dependencies: MetroFare
# Basic Setup
Creating a Vending Machine
<br>
Place a sign with the following format:
- Line 1: [jdhbk] (Customizable in Config)
- Line 2: Your company/store name

# Claiming Ownership
To claim a vending machine:
````
  /jdhbk register
````

# Commands
## General Commands:
Aliases of /jdhbk:
````
/vnd, /jidouhanbaiki, /vendingm, /jdh
````
Claim ownership of the new vending machine you're looking at:
````
/jdhbk register
````
Check the owner of the vending machine you're looking at
````
/jdhbk owner
````
Remove your ownership from the vending machine
````
/jdhbk deregister
````
Transfer ownership to another player
````
/jdhbk assign <player>
````
## Item Management:
The slot number was assigned as below:
<br>
![alt text](https://i.imgur.com/gK9plGo.png)
<br>
The vending machine uses specific slot numbers in its GUI:
<br>
Row 2: Slots 10-16
<br>
Row 3: Slots 19-25
<br>
Row 4: Slots 28-34
<br>
Row 5: Slots 37-43
<br>
Use these slot numbers when managing your items.
### Main Page:
![alt text](https://i.imgur.com/HDAdYVs.png)
<br>
Add an item to a slot, the amount of items you would like to sell depends on the amount of items you are holding:
````
/jdhbk create <slot> <price> [display name]
````
Remove an item from a slot
````
/jdhbk remove <slot>
````
Change an item's display name
````
/jdhbk rename <slot> <name>
````
Change an item's price
````
/jdhbk price <slot> <price>
````

## Configuration
![alt text](https://i.imgur.com/vcJB4Iy.png)
<br>
The block pointed by red arrow will be changed
<br>
Set blocks for payment processing
- Normal block: Shows when waiting for payment
- Success block: Appears when payment is completed
````
/jdhbk material <normal block> <success block>
````

# Using the Vending Machine
## As a customer
1. Right-click on the vending machine sign
2. Browse available items in the GUI
3. Click on an item to purchase it
4. The system will automatically process payment using the DebitCard system
5. Receive your item once payment is confirmed
## As an owner
1. Claim the vending machine with /jdhbk register
2. Add items with /jdhbk create while holding the item
3. Set appropriate prices for your items
4. Configure payment blocks with /jdhbk material
5. Manage your items using the various management commands
## Reminders
- Please use the vending machine one by one instead of using multiple of them at one time
- Purchase after the "success block" disappears or else error may occur.
