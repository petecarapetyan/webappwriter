# webappwriter
Source for rocket SSG - webappwriter.com

## STUFF I DID:

- copied relevant stuff from rocket-template
- - docs/_assets
- - docs/_includes
- - docs/_data
- made relevant changes to above files 
- - by inspecting each
- - also created/imported/yada necessary other files such as icons
- ran `firebase init`
- - selected only hosting
- - pointed to correct instance (webappwriter in this case)
- - set public dir to `_site`
- fixed build in package .json `"build": "rocket build"`
- added `"deploy": "npm run build && firebase deploy"`