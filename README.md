# AW Shared Project

# clone repo
git clone https://github.com/heiner-ulrich/awShared.git


# enable devhub in org

# authorize devhub
sfdx auth:web:login --setalias my-sandbox
sfdx auth:web:login --setdefaultdevhubusername --setalias my-hub-org 

# enable source tracking and packaging


# create scratch
sfdx force:org:create --definitionfile config/project-scratch-def.json --durationdays 30 --setalias aw-shared-ayo -v AW-org
sfdx force:config:set defaultusername=aw-shared 
sfdx force:org:open -u test-njpub1b4oghp@example.com