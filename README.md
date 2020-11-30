# Training Repository Template
This repository holds documentation on how to create an Application development training repo  

{% include list.liquid all=true %}

## What to include ##
Include a project description as above, as well as the script that lists all sub md files

Include your sub .md files at the root of this repo in the following fashion:
* Configure the project
* Implement the project
* Run the project
Those will end up listed in the description and browsable in a "tutorial manner" thanks to the liquid script above

If you have project specific items to document, add it here as done for the Submodule doc below

Finally, document that README with the documentation and disclaimer from Silicon Labs repos 

## Adding and Updating this repo as a submodule in the main doc centralization ##
###### Fork the master documentation repo
Fork [this repo](https://github.com/Jerome-Silabs/SE_FAE_team.git) and work on this
Push changes by creating a pull request

###### Submodule create 
To add a new training app to the main documentation repo, create a git based on this template
Then simply call from the root of teh main repo:

```
git submodule add https://github.com/brian-silabs/Z3_RollerShutter.git .\zigbee\Z3_RollerShutter
```

This will attach your app repo at this current state to the main documentation one

###### Submodule update
In order to update the main repo after changes have been made to the submodule

```
cd .\zigbee\Z3_RollerShutter\
(git checkout main)
git pull
cd ../..
git add .\zigbee\Z3_RollerShutter\
git commit -m "Updated submodule"
git push
```

## Documentation ##

Official documentation can be found at our [Developer Documentation](https://docs.silabs.com/zigbee/latest/) page.

## Disclaimer ##

The Gecko SDK suite supports development with Silicon Labs IoT SoC and module devices. Unless otherwise specified in the specific directory, all examples are considered to be EXPERIMENTAL QUALITY which implies that the code provided in the repos has not been formally tested and is provided as-is.  It is not suitable for production environments.  In addition, this code will not be maintained and there may be no bug maintenance planned for these resources. Silicon Labs may update projects from time to time.

