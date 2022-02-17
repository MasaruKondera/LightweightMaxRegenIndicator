# HowTo: Install this modification

Warning: This mod is not compatible out of the box with mods that also edit the own_ship_health.unbound file.

**1. Copy the "res_mods" folder**  
Just copy the res_mods folder from this release into the latest version directory from WoWs located in the bin folder.  
It will look similar to this: 
```
C:\World_of_Warships\bin\5045210
```

If it asks you to overwrite the own_ship_health.unbound file, then continue with the HowTo: Patch your own unbound file
section of this Readme file.


---

# HowTo: Uninstall this modification

**1. Delete the following file**  
_Warning: Only delete these files in case you haven't patched your own_ship_health.unbound file. If you have patched
your file, then continue with Step 2._

```
/gui/unbound2/mods/own_ship_health.unbound
```

**2. Restore your own_ship_health.unbound backup**
Replace the own_ship_health.unbound file with your backed up version.

Now you have uninstalled the mod successfully.

---

# HowTo: Patch your own own_ship_health.unbound file

In this tutorial I will try to explain, how to make your existing modification compatible
with this modification.

## Preparations
&emsp;Create a backup of the already existing own_ship_health.unbound file which you want to modify.
## Patching the own_ship_health.unbound
**1. Open the own_ship_health.unbound with an editor of your choice**  


**2. Check if OwnHealthBarRegen is defined**  
Check if the line below can be found in the own_ship_health.unbound file you want to modify.
If it doesn't exist continue with step 3. Otherwise advanced knowledge is needed to get both mods compatible.

```
(def element OwnHealthBarRegen (_entityId:number = 0) layout=true
```

**3. Copy the entire content of own_ship_health.unbound**  
Copy the content from this modification into the already existing mod file. 