### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Pass the dinosaur!

## Step 1
You need to sneak past the dinosaur by making yourself invisible. Can you make this happen? 


### ~ tutorialHint
If you are on a Windows device, try pressing shift and W to sneak in Minecraft.  


```ghost
player.onTravelled(SNEAK, function () {
    mobs.applyEffect(INVISIBILITY, mobs.target(NEAREST_PLAYER), 3, 1)
})
```