# Origins MCDOC

<img width="1856" height="512" alt="origins_mcdoc_banner" src="https://github.com/user-attachments/assets/a0dfe0fd-c671-4467-b40e-5ec9e25c0546" />

Definition files using the schema format, [`mcdoc`](https://github.com/SpyglassMC/Spyglass/tree/main/packages/mcdoc), for describing data structures used by [Minecraft Origins](https://modrinth.com/mod/origins), including its CODECs, JSONs, and NBTs

<img width="1500" height="500" alt="showcase" src="https://github.com/user-attachments/assets/b2dc2c84-8e40-4284-9ea2-0f1a1f962ddb" />

## Dependencies
- [Datapack Helper Plus](https://marketplace.visualstudio.com/items?itemName=SPGoding.datapack-language-server) (Visual Studio Code extension) from [Spyglass](https://github.com/SpyglassMC/Spyglass) project by SPGoding

## Instalation and Recommended Configuration 

1. ⬇️ Download the whole repository, either:
    - via [**git tool**](https://github.com/git-guides/install-git): [`git clone`](https://github.com/git-guides/git-clone) and (easier to update, via [`git pull`](https://github.com/git-guides/git-pull))
    - **OR** `Code -> Download ZIP` on Github, and extract `zip` archive *(rearange the folder structure if needed, so the `java` folder is directly inside of it)*
2. 💡 Put the folder with **Origins MCDOC** somewhere, you will remember
3. ➕ While having any datapack or workspace with datapacks open in Visual Studio Code:
    1. Go to `File -> Add Folder to Workspace...`
    2. Navigate and select the **Origins MCDOC** folder you stored somewhere in **step 2.**
    3. In the *"EXPLORER"* tab on the left, drag and the newly added folder **above** the top folder of your workspace *(Spyglass searches only the root folder of the workspace for `spyglass.json` file and mcdoc inside it recursively)*. **See the gifs below for a demonstration of configuration!**

<img width="1000" height="500" alt="downloadin_zip_file" src="https://github.com/user-attachments/assets/21148ad3-9c09-4404-b57b-73aab705f8d8" />
<img width="375" height="250" alt="add_to_workspace1" src="https://github.com/user-attachments/assets/90b72a5d-34fc-4ac4-b9bc-829ad1d986ad" />
<img width="375" height="250" alt="add_to_workspace2" src="https://github.com/user-attachments/assets/2c193525-8edd-4718-a81c-5f1e611890cc" />

## Supported Versions
- **`1.20.1`** - *experimental*
- **`1.20.2`** - full support
- **`1.20.4`** - full support
- **`1.21.1`** - full support

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
- Support for `*:*` identifier syntax
- Making `origins:multiple` unable to be defined as subpower type inside another `origins:multiple`
- Registering of "origins:multiple" subpowers in power resource, so it can be referenced from actions like `origins:grant_power`
- Some field requirements are not met (ex. in `apoli:damage` one of `amount`, `modifier`, `modifiers` should be defined, in the meantime all are just set to optional).
- Alias fields, which are currently not supported my mcdoc (making them required is impossible, same with making two field names mutually exclussive)
- Support for cardinal component `nbt`
- Support for texture/model/shader paths auto-completing
- Support for particle params syntax of [Particle Effect](https://origins.readthedocs.io/en/latest/types/data_types/particle_effect/) data type
