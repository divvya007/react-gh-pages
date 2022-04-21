
# How to deploy Create React App

## Steps to follow

1.  In your terminal run this command to install gh-pages as “dev-dependency”, which will allow you to create a new branch on your GitHub repo:

        <b>npm install gh-pages --save-dev<b/>

2. Go to your package.json file and add
      <b>"homepage": "https://username.github.io/repository-name"</b>, at the top level
   which looks something like this :
   
  ![Screenshot 2022-04-21 2 23 10 PM](https://user-images.githubusercontent.com/40967002/164472028-5247996e-d885-4f7e-bded-f536cb19fb60.png)


3. Now again in package.json add to your scripts
   <b>"predeploy": "npm run build"<b/> ,
   <b>"deploy": "gh-pages -d build"</b>
   
  ![Screenshot 2022-04-21 2 26 16 PM](https://user-images.githubusercontent.com/40967002/164472374-951758b0-5ed1-4c30-85ac-0dd249e9a5a9.png)
 
   

4. Last but not the least save package.json, and run the following command to deploy it to GitHub Pages:

      <b>npm run deploy<b/>

5 Your branch is now published.
