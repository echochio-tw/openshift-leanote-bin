# Custom MongoDB cartridge for OpenShift from https://github.com/icflorescu/openshift-cartridge-mongodb
# include leanote-bin code

![mongodb-openshift](https://cloud.githubusercontent.com/assets/581999/13374624/f9509bc2-dd92-11e5-8068-a87c9c3f6312.png)

This is a custom OpenShift cartridge providing MongoDB 3.4.x + leanote-bin web



rhc create-app leanote diy  https://raw.githubusercontent.com/chio-nzgft/openshift-leanote-bin/master/metadata/manifest.yml

rhc cartridge stop icflorescu-mongodb-3.4.1 --app leanote

rhc cartridge start icflorescu-mongodb-3.4.1 --app leanote

# create app

    rhc create-app leanote diy  https://raw.githubusercontent.com/chio-nzgft/openshift-leanote-bin/master/metadata/manifest.yml
    
# restart mongodb to build leanote web

    rhc cartridge restart icflorescu-mongodb-3.4.1 --app leanote


