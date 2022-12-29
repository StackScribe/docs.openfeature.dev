# Contribute to the OpenFeature documentation

## Building the documentation locally

You should build the documentation from your branch
and check that the formatting is correct before pushing your PR.

To set this up:

1. [Should one `checkout -b` a new branch before doing this?
   I did not but I now have changes in my local main branch,
   which is why this PR is against main, which I realize is a no-no.]

1. Download the appropriate version of `Node.js`
   from the Node.js [download](https://nodejs.org/en/download/) page.

1. Install `Node.js` following the instructions on the
   [Installing Node.js via Package Manager](https://nodejs.dev/en/download/package-manager/) page.

1. Install `yarn` following the instructions on the
   [How to Install and Use the Yarn Package Manager for Node.js](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-the-yarn-package-manager-for-node-js) page.

   Just for clarity, these are the commands I ran:
   ```
   cd docs.openfeature.dev/
   brew install node
   node -v
   sudo npm install -g yarn
   yarn --version
   yarn set version berry
   yarn --version
   yarn install
   yarn
   yarn start
   ```

   The output of the last command gives an error:
   ```
   yarn start
   [INFO] Starting the development server...
   Copying external content for 'spec'.
   [ERROR] Error: ENOENT: no such file or directory, lstat '/Users/meg.mcroberts/Code/docs.openfeature.dev/external-content/specification/specification'
   [INFO] Docusaurus version: 2.2.0
   Node version: v19.3.0

   ```

