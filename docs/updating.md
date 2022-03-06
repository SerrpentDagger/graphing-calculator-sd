## Updating GCSD

A given release will have a combination of symbols/keywords from below.
Each is a straightforward instruction for what needs to be copied from the new version to your current installation.
My reccommendation for updating is to download the new version's .zip file, extract it into a convenient directory, and then follow the instructions indicated by the symbols/keywords.
You can then delete the remaining portions of the new installation, since you've updated the old one.

### Symbols
- \*: Required in order for the update to work.
- ^: Recommended for non-essential, visual asset improvements. Replaces old assets.
- +: Recommended for non-essential, visual asset additions. Adds new assets.

### Keywords
- jar: Replace the current 'GraphingCalculator...jar" file with the new one.
- \<data folder name\>: When the name of a folder in 'data/' is written, the instruction is to merge the new 'data/\<name\>' folder with the old one by dragging the new one into 'data/'. If the ^ symbol is present, replace the old conflicting files when prompted, unless they're ones you've added yourself and want to keep.

### Examples
- \*jar ⠀*⠀(The old jar should be replaced with the new one, and doing so is required in order for the update to work.)*
- ^themes ⠀*⠀(Merge the new 'data/themes' folder with the old one by dragging the new one into the old 'data/' folder. Replace conflicts. Not functionally required, but provides visual improvements.)*
- +textures ⠀*⠀(Merge the new 'data/textures' folder with the old one by dragging the new one into the old 'data/' folder. Replacing conflicts is unnecessary, since they should be identical. Not functionally required, but provides new visual assets.)*
- ^+skyboxes ⠀*⠀(Merge the new 'data/themes' folder with the old one by draggin the new one into the old 'data/' folder. Replace conflicts. Not functionally required, but improves old assets and adds new ones.)*
