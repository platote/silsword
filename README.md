# Silsword

The Silsword comes in a very high quality crafting. It damages NPCs, its environment and comes with special shaders effects (a blood trail following each slices)

- [Silsword](#silsword)
- [Base .scn configuration](#base-scn-configuration)
- [Description](#description)
- [Customize the 3D Model](#customize-the-3d-model)
- [Issues](#issues)

![](https://i.imgur.com/QqjePWi.png)

# Base .scn configuration
You can copy & paste it into your .scn file to get the silsword working **as-is**
```json
    {
      "position": [
        0,
        0,
        0
      ],
      "start_url": "https://webaverse.github.io/silsword/"
    }
```

# Description 
- The "wear" component ensures atatchement to the spine.
![](https://i.imgur.com/Bvc2uvS.png)
- The "aim component" helps you aim an enemy before you slice it 
![](https://i.imgur.com/XwszLI3.png)
- Avatars can swing it like a sword, because of the "use" component. 
![](https://i.imgur.com/b5M3pBh.png)



# Customize the 3D Model 

![](https://i.imgur.com/RMXTrsD.png)

In order to change the model displayed, go to [index.js](https://github.com/webaverse/silsword/blob/main/index.js), and at line 622, change "megasword_v4_texta.glb" for your model (A reference of the process can be found [here](https://webaverse.notion.site/Creating-Weapons-765b54dd5b4041969cbbd59f7fd23ac7))

```javascript
e.waitUntil((async () => {
    let u2 = baseUrl + 'megasword_v4_texta.glb';
    if (/^https?:/.test(u2)) {
      u2 = '/@proxy/' + u2;
    }
```

# Issues
No issues encountered during test, works as intented