# Overview
Few useful Blender operators inside one addon script. Especially useful for improving imported MMD models bone hiearchy. Made for lovely VRChat community.

# Installation
1) Download https://raw.githubusercontent.com/netri/blender_neitri_tools/master/neitri_tools.py (ctrl+s)
1) In Blender go to: File > User Preferences > Add-ons > 
    1) Install Add-on from File.. > Find and Select just downloaded file "neitri_tools.py"
    1) Select Testing > Object: Neitri's Tools > tick to enable
    1) Save User Settings

# Environment
Created and tested in Blender v2.79

# Usage
Adds into space menu following operators:

* Delete Zero Weight Bones and Vertex Groups - Useful to cleanup MMD model bone hiearchy, because they usually come with alot of extra bones that don't directly affect any vertices. Less bones means faster import times into Unity and results in more optimized model.
<br> ![](https://i.imgur.com/x3KVvG3.gif)

* Delete Bones Constraints - Useful if you chracter is now stuck in weird pose, it is probably because of Bones Constraints that worked well with IK bones you just deleted in "Delete Zero Weight Bones and Vertex Groups".

* Delete Bone and Add Weights To Parent - Useful to remove any weighted bones, because you usually want to add their weights to their parent. MMD models usually come with few twist bones to better simulate real life human anatomy, however Unity nor VRChat support those. It's better to get rid of them, while deleting them you ideally want their weights to be added to their parent bone.
<br> ![](https://i.imgur.com/Woddyu2.gif)

