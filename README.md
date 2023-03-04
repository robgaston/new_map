# New Map

## Getting Started
Install the following dependencies:
- [Node.js](https://nodejs.org/)

You'll also need a Git client & text editor; if you don't have those, then you should also install the following:
- [Git](https://git-scm.com/downloads)
- [VS Code](https://code.visualstudio.com/)

You'll also want to [sign-up for Mapbox services here](https://www.mapbox.com/signup/) and, if you haven't already, [create a GitHub account](https://github.com).

After installing git, configure it by running:
```sh
git config --global user.name "<your name>"
git config --global user.email "<your email>"
```

Now you can use this template repository to start building your own web map:
- Use this template to create a new repository
- Install the [GitHub Pull Requests and Issues VSCode Extension](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
- [Sign into GitHub with VSCode](https://code.visualstudio.com/docs/sourcecontrol/github#_getting-started-with-github-pull-requests-and-issues)
- [clone the repository](https://code.visualstudio.com/docs/sourcecontrol/github#_cloning-a-repository) you've created from this template in GitHub using VSCode

After cloning the repo, you'll need to insert your Mapbox public access token ([which can be found here](https://www.mapbox.com/account/)) into [`src/settings.json`](https://github.com/robgaston/new_map/blob/main/src/settings.json#L3).

You'll also need to install your package dependencies locally by running the following from the root directory of your cloned repository:
```
npm install
```

## Development
To run the app locally, run the following from the root directory of your cloned repository:
```
npm start
```

The application should now be running at http://localhost:1234/

Changes that you make to javascript and CSS files will be automatically refreshed!

## Building
Before deploying, you must first build the website by running the following command from the root directory: 
```
npm run build
```

## Deployment
To deploy your latest code to the web, simply build (as per above) then commit and push your local changes to the `main` branch in Github.
