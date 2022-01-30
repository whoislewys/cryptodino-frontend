pros/cons of isolating dino sprite

pro:
* simpler to reason about dino sprite
* 

cons:
* add a little complexity to code



could move dino sprites to END of sprite sheet, leave everything else in place


how do you design the nfts then?
nft structure:
{
  spritesheet: '<link>',
}

{
  components: [
    'head': 'hat',
    'eye': 'monocle',
    'chest': null,
    ''
  ]
}



tradeoffs:

standalone spritesheet:
* more flexibility for different additions while keeping hitboxes same
* could expand to different sprites entirely with differrent hitboxes
* kind of necessary for animated additions (e.g. chain moving when dino ducks down)
* feels easier

components: 
* harder to render
* for animated components (e.g. animated chain) you need to create a sprite sheet for each component

k so nfts should definitely be standalone spritesheet, meaning dino should definitely be isolated into it's own sheet


