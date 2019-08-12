- Install _git_, _node_ & _npm_
- Create a new _GitHub_ repository
- Copy the clone url
- Open a command line tool and navigate to a "parent folder"
- Clone your repository; run `git clone https://github.com/<username>/<repository>.git`
- Create a simple _React_ application; run `npx create-react-app <repository>`
- Navigate to the projects folder; run `cd <repository>`
- Install the _GitHub Pages_ package as a developer dependency; run `npm i --save-dev gh-pages`
- Configure _GitHub Pages_ in your project:
  ```
  {
    ...
    "homepage": "https://<username>.github.io/<repository>",
    "scripts": {
      "predeploy": "npm run build",
      "deploy": "gh-pages -d build"
    }
  }`
  ```
- Go to the "Settings" tab of your _GitHub_ repository and make sure that the `gh-pages branch` is selected under _GitHub Pages_ "Sources"
- Go to your new site at https://<username>.github.io/<repository>/
