# origins-mcdoc

Mcdoc for mod Origins - definition files using the schema format, mcdoc, for describing data structures used by Minecraft Origins mod, including its CODECs, JSONs, and NBTs

## Dependencies
- Datapack Helper Plus by Spyglass (vs code extension)

## Credits
The whole "resources" directory contains data types from other repositories, and owned by their respective owners!
These embeded data types include:
- [Origins](https://github.com/apace100/origins-fabric)
- [Apoli](https://github.com/apace100/apoli)

Reference mcdoc used: https://github.com/SpyglassMC/vanilla-mcdoc

Big thanks to people from Spyglass discord server who helped me to deal with problems with mcdoc!

## How to use
Currently the only way is either:
- downloading the whole repository and putting it in the datapack's folder, either:
  - via `git clone` command
  - **OR** `Code -> Download ZIP` on Github
- **OR** downloading it somewhere on your computer and adding it to the workspace, via `File -> Add Folder to Workspace...` and selecting it

## Features
The syntax checking includes all data types defined in Origins mod:
- JSON
  - Badge JSON
  - Global Power Set JSON
  - Origin JSON
  - Origin Layer JSON
  - Power JSON
- General Types
  - Badge Types
  - Keybindings
- Commands
  - Origins
  - Pehkui (most of them)
- Power types
- Action types
- Condition types
 
## Problems:
- power type "origins:multiple" can be defined as subpower type.
- subpowers of a "origins:multiple" power type are not registered as a power resource.
- Some field requirements are not met (ex. in `apoli:damage` one of `amount`, `modifier`, `modifiers` should be defined, in the meantime all are just set to optional).
- alias fields are not supported my mcdoc (making them required is impossible, same with making both names mutually exclussive)

## Future:
- add cardinal component nbt
- support for texture/model/shader paths auto-completing
- support for particle params syntax
- support for earlier versions
- Fabric load conditions
- (maybe) add versioned comments (changes in 1.21)
