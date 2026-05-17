# Origins MCDOC

<img width="1856" height="512" alt="origins_mcdoc_banner" src="https://github.com/user-attachments/assets/a0dfe0fd-c671-4467-b40e-5ec9e25c0546" />

Definition files using the schema format, [`mcdoc`](https://github.com/SpyglassMC/Spyglass/tree/main/packages/mcdoc), for describing data structures used by [Minecraft Origins](https://modrinth.com/mod/origins), including its CODECs, JSONs, and NBTs

## Dependencies
- [Datapack Helper Plus](https://marketplace.visualstudio.com/items?itemName=SPGoding.datapack-language-server) (Visual Studio Code extension) from [Spyglass](https://github.com/SpyglassMC/Spyglass) project by SPGoding

## Instalation
1. Download the whole repository and putting it in the datapack's folder, either:
  - via `git clone` command
  - **OR** `Code -> Download ZIP` on Github
- **OR** downloading it somewhere on your computer and adding your datapack to the workspace, so:
  1. Open the folder with origins-mcdoc in vs code
  2. Add your datapack to the workspace via `File -> Add Folder to Workspace...`
  
<img width="1499" height="743" alt="downloadin_zip_file" src="https://github.com/user-attachments/assets/21148ad3-9c09-4404-b57b-73aab705f8d8" />

## Credits
The whole "resources" directory contains data types from other repositories, and owned by their respective owners!
These embeded data types include:
- [Origins](https://github.com/apace100/origins-fabric)
- [Apoli](https://github.com/apace100/apoli)
- [Fabric API (convention tags)](https://github.com/FabricMC/fabric-api/tree/HEAD/fabric-convention-tags-v2/src/generated/resources)
Reference mcdoc used:
- https://github.com/SpyglassMC/vanilla-mcdoc
Big thanks to people from Spyglass discord server who create this wonderfull project and helped me to deal with problems with mcdoc!

## Future features:
- Making `origins:multiple` unable to be defined as subpower type inside another `origins:multiple`
- Registering of "origins:multiple" subpowers in power resource, so it can be referenced from actions like `origins:grant_power`
- Some field requirements are not met (ex. in `apoli:damage` one of `amount`, `modifier`, `modifiers` should be defined, in the meantime all are just set to optional).
- Alias fields, which are currently not supported my mcdoc (making them required is impossible, same with making two field names mutually exclussive)
- Support for cardinal component `nbt`
- Support for texture/model/shader paths auto-completing
- Support for particle params syntax of [Particle Effect](https://origins.readthedocs.io/en/latest/types/data_types/particle_effect/) data type
- *Fabric load conditions
