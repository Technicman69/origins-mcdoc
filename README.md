# origins-mcdoc

Mcdoc for mod Origins - definition files using the schema format, mcdoc, for describing data structures used by Minecraft, including its CODECs, JSONs, and NBTs

Dependencies: Datapack Helper Plus by Spyglass (ofc)


## Credits
The whole "resources" directory contains data types from other repositories, and owned by their respective owners!
These embeded data types include:
- [Origins](https://github.com/apace100/origins-fabric)
- [Apoli](https://github.com/apace100/apoli)

Reference mcdoc used: https://github.com/SpyglassMC/vanilla-mcdoc

## How to use
Currently the only way is either adding whole repo to the workplace or putting it in the datapack's folder
I don't know any other way how to include dependencies yet. Imma ask Misode in the future

## Features
The syntax checking currently includes data types and files listed below:
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
- Origin keybinds need to be injected into vanilla ones (or modded keybinds need to be defined)
- power type "origins:multiple" shouldn't be a subpower.
- subpowers of a "origins:multiple" power type are not registered as a power resource.
- Versioning is all wrong (support for #[since] and #[until] attributes in dispatch keys in `.mcdoc` language needed)

## Future:
- specify which power types don't have condition fields
- Alias fields
- support for texture/model/shader paths
- support for particle params syntax
- support for 1.21
- support for earlier versions
- Fabric load conditions
