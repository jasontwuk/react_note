# React Note

## Deploy A React Project to Github:
Make sure you have already **built** a repository on Github and **pushed** your React app code to it.

### Step1: install the `gh-pages` dependency in package.json 
`npm install gh-pages - save-dev`

![Screenshot 2021-02-25 at 20 02 56](https://user-images.githubusercontent.com/13745974/109210392-a61a1080-77a4-11eb-9358-df9b45fe334a.png)

### Step2: add "homepage" property to package.json
`"homepage": "http://{username}.github.io/{repo-name}"`

![Screenshot 2021-02-25 at 19 46 52](https://user-images.githubusercontent.com/13745974/109208639-74a04580-77a2-11eb-90ba-b5059fa95321.png)

### Step3: add scripts in package.json
"scripts": {<br/>
// ...<br/>
`"predeploy": "npm run build",`<br/>
`"deploy": "gh-pages -d build"`<br/>
}

![Screenshot 2021-02-25 at 19 53 42](https://user-images.githubusercontent.com/13745974/109209362-5dae2300-77a3-11eb-9ec5-aec1c98318b4.png)

### Step4: deploy it to Github
In terminal: type `npm run deploy`

![Screenshot 2021-02-25 at 19 59 33](https://user-images.githubusercontent.com/13745974/109210001-27bd6e80-77a4-11eb-9ecf-f976b63afa19.png)

After it is done, a new branch named `gh-pages` will be created in your respository.

![Screenshot 2021-02-25 at 20 10 54](https://user-images.githubusercontent.com/13745974/109211117-b088da00-77a5-11eb-8404-76be1b067029.png)

### Step5: set up your GitHub Pages live site
Go to {your-repository} --> Setting --> GitHub Pages section, then select `gh-pages` as your branch and press "Save" button.<br/>
Wait for a bit, then you can see your React app up and running.

![Screenshot 2021-02-25 at 20 21 39](https://user-images.githubusercontent.com/13745974/109212371-57ba4100-77a7-11eb-8d32-f7350458667c.png)
