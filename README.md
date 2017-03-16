# Custom MongoDB cartridge for OpenShift 
# from https://github.com/icflorescu/openshift-cartridge-mongodb
# include leanote-bin code

# This is a custom OpenShift cartridge providing MongoDB 3.4.x + leanote-bin web

rhc create-app leanote diy  https://raw.githubusercontent.com/chio-nzgft/openshift-leanote-bin/master/metadata/manifest.yml

rhc cartridge stop icflorescu-mongodb-3.4.1 --app leanote

rhc cartridge start icflorescu-mongodb-3.4.1 --app leanote

# create app

    rhc create-app leanote diy  https://raw.githubusercontent.com/chio-nzgft/openshift-leanote-bin/master/metadata/manifest.yml
    
# restart mongodb to build leanote web

    rhc cartridge restart chiotest-mongodb-3.4.1 --app leanote


