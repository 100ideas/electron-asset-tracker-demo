meteor webapp that stores and displays gps tracks collected from a particle.com/electron and asset tracker kit.

based on [campaign-hawk meteor tutorial](https://medium.com/@SamCorcos/building-campaignhawk-with-meteor-and-react-part-2-d4551708dcde#.k70d0z9lv).


### settings.json

Sign up for a [mapbox](http://mapbox.com) developer account to get an access token, then put the token in `settings.json`. Tell meteor to use this file in development or production with `meteor --settings settings.json`.

I initialized the settings.json file with dummy data, then untracked it from git. You may need to follow the same steps so you don't publish your secret keys (although the project .gitignore should be telling git not to track it). Here's what I did:

```
git add settings.json
git commit -m "added settings.json with dummy data"
git push origin master

// Stopped tracking, then added secret keys
git update-index --assume-unchanged settings.json
```
