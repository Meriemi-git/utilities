# utilities
This repository will include many various things.

Each branch will refer to a tool or a script and documentation section of readme will change according to the tool.

## Documentation

### gen-se-policies.sh
Script to generate .se policy files from adb logs for custom Android ROM.

### Installation
On Arch : 
`$ yay gen-se-policies`

On other distributions :
Copy the .sh on your computer and add execution rights on it with:

`$ chmod +x gen-se-policies.sh`
Call the script with the right params:

`$ ./gen-se-policies.sh -i adb.log -d lineage/device/your_phone/devie_code/se_policies/vendor`

This script take 3 arguments:

- -i (required) : path to the adb log file
- -d (optionnal) : destination where the script will create or update the .se files
- -f (optionnal) : generate one only .txt file conatining all generated rules 

If you specified a destination folder that contains existing .se files the script will add rules on it only if rule not already exists.

