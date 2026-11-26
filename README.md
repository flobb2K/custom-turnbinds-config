# flobb's turnbinds
# Turnbinds with customizable turnspeeds for CS2/CSGO

This config uses a workaround to add the legacy console variables `cl_yawspeed` and `cl_pitchspeed` from ***Counter-Strike: Source*** to the latest game in the series, ***Counter-Strike 2***, and also its predecessor, ***Counter-Strike: Global Offensive***, <ins>using only console commands</ins>. It also adds a multitude of different <ins>binds and customization</ins> options that allow full use of these long-lost but not forgotten console commands.

## Features
### cl_yawspeed
This config allows the user to **change yawspeed** by entering `cl_yawspeed_[value]` into the developer console or executing `.cfg` files.
>[!IMPORTANT]
>`cl_yawspeed` is measured in **degrees per second** and can be set to any whole number from `1` to `300`.

### cl_pitchspeed
This config allows the user to **change pitchspeed** by entering `cl_pitchspeed_[value]` into the developer console or executing `.cfg` files.
>[!IMPORTANT]
>`cl_pitchspeed` is measured in **degrees per second** and can be set to any whole number from `1` to `45`.

### Fixed Binds
**Bind** as many **keys** as you like **to different** `cl_yawspeed`/`cl_pitchspeed` **commands**!  

`bind "[key]" "cl_yawspeed_[value]"`  
`bind "[key]" "cl_pitchspeed_[value]"`

### Toggle/Cycle Binds
- **Cycle between** two, three, or four **different** `cl_yawspeed` **settings** using **a single key**!
- **Cycle between** two or three **different** `cl_pitchspeed` **settings** using **a single key**!
- **Pair** Fixed Binds with Toggle/Cycle Binds so that the Fixed Binds **also affect the cycle** alias!
- Optionally **reset the** `cl_yawspeed` **cycle** alias automatically **whenever** you **reset** your **stage or run**!

### Hold-to-Activate Binds
Hold-to-Activate Binds **must be held down** to change the `cl_yawspeed` setting.  
**While none of these binds is held**, a customizable default `cl_yawspeed` setting is active.  
This config supports up to three Hold-to-Activate Binds, which, together with the default setting, give you up to four different speed settings.  

>[!IMPORTANT]
>Hold-to-Activate Binds **cannot be combined with** Fixed Binds or Toggle/Cycle Binds!

### Visual Feedback
- **HUD** color change
- **crosshair** color change
- **both HUD and crosshair** color change
- 10 different colors for all of the above

>[!NOTE]
>For the **crosshair color change** to work in ***Counter-Strike: Global Offensive***, you need to **edit the** `turnbinds\setup\setup.cfg` **file**.   
>See that file for further instructions.

### Sound Effects
- Add **sound effects** to your binds!
- Choose from **21 different** sounds!

>[!NOTE]
>**Any** sound file from the game files of CS2/CS:GO, including music kits, **can be added** as a sound effect **using the** `turnbinds\setup\setup.cfg` **file**.
>See that file for more information.

### Full Readability
**I'm not keeping any secrets here**. Every single config file has its own header explaining its use and I did my best to make everything **easy to read and understand**.

### Full Customization
In the included `turnbinds\settings.cfg` file, I have provided **many customization options** so that you can make this **your very own** config. 
If you have tinkered with Counter-Strike configs before and want to add more features yourself, I also recommend checking out the `turnbinds\setup\setup.cfg` file.

## How to use
1. Download the `.zip` file containing the config files under "Releases".
2. Extract all files from the `.zip` archive.
3. Choose your preferred language for the config files and open the corresponding folder.
4. Inside, you will find the `turnbinds` folder. Copy this folder, including all of its contents, to  
   `[Drive]:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg`
5. Set up the config using the `settings.cfg` file in the `turnbinds` folder.
6. To execute the config, type `exec turnbinds\exec.cfg` into the developer console. The screenshot shows what it should look like afterwards.
7. For convenience, I recommend binding the exec command to a key: `bind "[key]" "exec turnbinds\exec.cfg"`
8. You can also add `exec turnbinds\exec.cfg` to your `autoexec.cfg` file.

<img width="2160" height="1440" alt="preview_screenshot" src="https://github.com/user-attachments/assets/86c1bc19-dbad-441e-8e74-61ae4351ca24" />

>[!NOTE]
>Your console **will not show** the confirmation text at startup **if you use** the autoexec method.

## Why should I use this config instead of external turnbind software?
### The advantages
- Far more options for creating binds
- Visual feedback
- Sound effects
- Uses only console commands
- Ability to change settings in-game using the developer console

### The drawback
Since `cl_yawspeed` and `cl_pitchspeed` do not actually exist as convars in-game, this config "emulates" them by modifying the `turnleft`/`turnright` and `turnup`/`turndown` commands. The downside is that you cannot change the turn speed while you are turning. For a turn speed change to take effect, you need to briefly stop turning and then start turning again.

## Special Thanks
- to INSPECTRO from Cybershoke for his advice on the `cl_yawspeed`/`cl_pitchspeed` commands
- to violetto for proofreading the Russian version

## Cybershoke
<img width="4100" height="475" alt="banner_cybershoke_anthrazit" src="https://github.com/user-attachments/assets/01df9424-7de2-40b0-8295-f4221597aebe" />
If you want to surf in CS2, I highly recommend Cybershoke. Their servers come with plenty of features, their maps are properly playtested, and the leaderboards are highly competitive.
