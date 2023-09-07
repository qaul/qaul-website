---
title: "Qaul Matrix Bridge"
preview: matrix_bridge.png
tags: 
---

# Bridge tutorial

### Requirements
You should have an account on matrix that can act as a bridge bot.

For more secure communications you can opt for running your own matrix homeserver but that is not necessary since our bridge works well on the default matrix server as well.

You should have the binary to the bridge either as code or distributed package.

We are still working on packaging the binary for end users and then in place of 
`cargo run –p qaul-matrix-bridge` you can simply run our binary.

### Initialization and Configuration
As of now, We are supporting the bridge only as a daemon process binary without any control on it via CLI or GUI. All the logics are integrated on matrix-sdk or ruma and qaul or libqaul.

On the server where you wish to start a binary between a local qaul network, You need to have one node running the binary and rest will follow along the way.

After installing the qaul project you can

```
cargo run -p qaul-matrix-bridge -h {homeserver_url} -a {bot-account} -p {bot-account-password} -f {feed_room_matrix_id}
```

- homeserver [-h or --homeserver] : The URL for matrix homeserver. Default can be [https://matrix.org]
- bot-account [-a or --account] : The user account of the bot on matrix. Eg : @qaul-bot:matrix.org then id is [qaul-bot]
- bot-account-password [-p or --password] : The password for your bot account on matrix
- feed_matrix_room [-f or --feed] : This option helps you to configure any one room as matrix

![image](https://user-images.githubusercontent.com/79367883/263565222-f7a89d53-6b25-47c8-a782-af373eb898e8.png)

### Inviting the Bridge to Matrix Room

Once the bridge is running up. You have to go to your own matrix account and create a new room. Please make sure to turn off any encryption. Now invite the bot to your matrix room and it automatically joins the room.

1. Create a matrix room and disable end to end encryption
![image](https://user-images.githubusercontent.com/79367883/263565281-a34806c4-4459-4199-a4af-7f95e7221ced.png)
2. Invite the bot account into the room ![image](https://user-images.githubusercontent.com/79367883/263565318-916c03d0-81fe-4e54-85c2-6e01ad0ff17c.png) ![image](https://user-images.githubusercontent.com/79367883/263565373-f642a6f0-89b3-4685-ba24-8d853a29ba6d.png) ![image](https://user-images.githubusercontent.com/79367883/263565387-011d0262-4903-4763-b850-879546864567.png)

# Navigating through Matrix Menu
We have multiple menu options available in our Matrix Menu. You can see the list of all the possible functionalities with !help command.
### !help 
![image](https://user-images.githubusercontent.com/79367883/263565468-8dc46247-6e73-4ab1-92af-776f846c9517.png)

### !qaul 
![image](https://user-images.githubusercontent.com/79367883/263565483-895fe092-26af-45e6-bc8e-969bb792274e.png)

### !users 
![image](https://user-images.githubusercontent.com/79367883/263565497-0a6b7706-a2bf-43d2-8bdf-afeefb866d8b.png)

### !invite 
![image](https://user-images.githubusercontent.com/79367883/263565511-92ae912c-de53-468a-8fc3-646bbe6894e2.png)
![image](https://user-images.githubusercontent.com/79367883/263565575-6b2d5315-cd39-4a43-8b21-7fa7b4168b79.png)
![image](https://user-images.githubusercontent.com/79367883/263565586-0ff5209d-8707-4a0c-8fb7-327687aeb603.png)
![image](https://user-images.githubusercontent.com/79367883/263565600-deaf8744-dfa8-4954-aa28-6f02b1383576.png)
![image](https://user-images.githubusercontent.com/79367883/263565605-18c3836a-d84b-4f84-9ca3-0903e152ac6e.png)

### !group-info
![image](https://user-images.githubusercontent.com/79367883/263565619-371b1d5b-306d-49be-81fb-201d1ef89620.png)

### !remove
![image](https://user-images.githubusercontent.com/79367883/263565632-76ae587f-a25d-4649-b655-e2d50b178e1b.png)
![image](https://user-images.githubusercontent.com/79367883/263565637-2583b0a3-45bd-4f0c-9b8e-ab0869822197.png)

# File Exchanges
![image](https://user-images.githubusercontent.com/79367883/263565656-5e1a5c95-454b-4aa3-9865-9873e537d17b.png)
![image](https://user-images.githubusercontent.com/79367883/263565663-98367dbb-83c0-4ce7-bbe1-8d994b977d2c.png)
