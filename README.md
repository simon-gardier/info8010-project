# info8010-project
Course page: https://github.com/glouppe/info8010-deep-learning
Project page: https://github.com/glouppe/info8010-deep-learning/blob/master/project.md
Project proposal: https://www.overleaf.com/7518417627ycrxkdktsnjc#f5cae5
project report: TBD

# Ideas

## Pitch
Tool to generate a texture pack for minecraft from a prompt.

## Dataset
- Scrap from websites
- Label each texture pack with its description from the website
- Generate more detailled labels for each item in the texture pack ? (Using a model to label them based on examples we would provide?)

## Training
- Text to Vectorization ?
- Vectorization to image ? 
- One model for each image ?

## Practical consideration
- Limit ourselves to 16x16 texture packs so each texture is only 256*3 = 768 features (256 pixels * RGB)
- Limit ourselves to a subset of items for with we generate the texture (e.g. do not generate the doors texture, mobs,... only generate the blocks textures)
- Will need a (hopefully) small script to then take these images and make a texture pack out of them (i.e. a rar file that can be imported in the `/ressourcepacks` forlder of Minecraft)

# Research
## Ressource pack websites to scrap
Website 1: https://www.curseforge.com/minecraft/search?page=1&pageSize=20&sortBy=relevancy&class=texture-packs
Website 2: https://www.planetminecraft.com/texture-packs/themed/?filter0=33&op0=1&monetization=0

## Text to Image
https://www.youtube.com/watch?v=w8YQcEd77_o
