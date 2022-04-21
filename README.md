# [deployment](https://divvya007.github.io/react-gh-pages/)

# How to deploy Create React App

## Steps to follow

1.  In your terminal run this command to install gh-pages as “dev-dependency”, which will allow you to create a new branch on your GitHub repo:

npm install gh-pages --save-dev

2. Go to your package.json file and add
   "homepage": "https://username.github.io/repository-name", at the top level
   which looks something like this :

image

3. Now again in package.json add to your scripts
   "predeploy": "npm run build",
   "deploy": "gh-pages -d build"

4. Last but not the least save package.json, and run the following command to deploy it to GitHub Pages:

npm run deploy

5 Your branch is now published
