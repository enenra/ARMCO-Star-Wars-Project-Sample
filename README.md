# ARMCO-Star-Wars-Project-Sample
A sample project on how to organize the ARMCO Star Wars Mod project.

# Setup
1. Download and install Github Desktop from here: https://desktop.github.com/ (All local Github functionality)
2. Create a Github account and contact me so I can add you as a collaborator.
3. Clone the repository to wherever you want: `File --> Clone repository...` and select the corresponding repository.
4. Run `Link to Mods Folder.bat` in any mod subfolder's Content\-folder to link that mod within the Space Engineers \Mods\ -folder. It will now appear as a regular folder within \Mods\ and is seen as that by Space Engineers as well.
5. If you want to remove a mod link from \Mods\ , run `Remove Link.bat` in the mod's subfolder.
6. Download and install SEWT: https://github.com/Gwindalmir/SEWorkshopTool/releases (Upload to Workshop)

# Upload
Within each mods subfolder are several bat files. Open `Update Thumbnail.bat`, `Upload to Workshop (Private).bat` and `Upload to Workshop.bat` with a text editor and adjust the paths for the variable SEInstallDir to your Space Engineers installation folder. (Mine is `C:\Program Files (x86)\Steam\steamapps\common\SpaceEngineers`, for example, thus the first line in those batch files will be `set SEInstallDir="C:\Program Files (x86)\Steam\steamapps\common\SpaceEngineers"`.

To update the thumbnail of the published mod, run `Update Thumbnail.bat`. It will automatically replace the thumbnail on the Workshop page with the thumbnail present in the mod's subfolder.

To upload or update the mod on the Workshop, run `Upload to Workshop.bat`. If you are uploading the first version of the mod, you can instead use `Upload to Workshop (Private).bat` to upload it set to private from the beginning.

# Work folders
Github specifically ignores all data inside `\[repository]\[mod-subfolder]\OriginalContent\`. Feel free to place any working files (such as FBX, etc.) within those folders. They will not be synchronized.

# Updating
If any changes are made to any file on github, simply open Github Desktop and click the "Fetch Origin"-button, and then click again for "Pull origin". That will synchronize any changes to your local folder and you will be able to test the latest changes without having to update a workshop mod.
