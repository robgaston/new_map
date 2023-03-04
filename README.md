# New Map Template

## Getting Started
Install the following dependencies:
- [Node.js](https://nodejs.org/)

You'll also need a Git client & text editor; if you don't have those, then you should also install the following:
- [Git](https://git-scm.com/downloads)
- [VS Code](https://code.visualstudio.com/)

After installing git for the first time, you'll need to configure it by running:
```sh
git config --global user.name "<your name>"
git config --global user.email "<your email>"
```

If you haven't already, you'll also need to create accounts for these services:
- [Mapbox](https://www.mapbox.com/signup/)
- [GitHub](https://github.com)

Now you can use this template repository to start building your own web map:
- Use this template to create a new repository
- Install the [GitHub Pull Requests and Issues VSCode Extension](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
- [Sign into GitHub with VSCode](https://code.visualstudio.com/docs/sourcecontrol/github#_getting-started-with-github-pull-requests-and-issues)
- [Clone the repository](https://code.visualstudio.com/docs/sourcecontrol/github#_cloning-a-repository) you've created from this template using VSCode
- Insert your Mapbox public access token ([which can be found here](https://www.mapbox.com/account/)) into [`src/settings.json`](https://github.com/robgaston/new_map/blob/main/src/settings.json#L3).
- Install the package dependencies by running the following from the root directory of your cloned repository:
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

You will need to [configure GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) to use the `main` branch and the `/docs` folder.
