# Custom MongoDB cartridge for OpenShift 
# from https://github.com/icflorescu/openshift-cartridge-mongodb
# include leanote-bin code

# custom cartridge providing MongoDB 3.4.x + leanote-bin web

# create app

    rhc create-app leanote diy  https://raw.githubusercontent.com/chio-nzgft/openshift-leanote-bin/master/metadata/manifest.yml
    
# restart mongodb to build leanote web

    rhc cartridge restart chiotest-mongodb-3.4.1 --app leanote


