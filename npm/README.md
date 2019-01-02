# Npm

`npm` makes it easy for JavaScript developers to share and reuse code. 

## Installation

npm is distributed with Node.js- which means that when you download Node.js, you automatically get npm installed on your computer. You can download the installer package [here](https://nodejs.org/).

To check if you have Node.js installed, run this command in your terminal:

```
node -v
```

You can install npm packages globally as `npm install <package_name> -g`

If you have an issue installing packages with error saying `Missing write access to /usr/local/lib/node_modules` run the command:

```
sudo chown -R $USER /usr/local
```