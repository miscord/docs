# How to install Node.js

The latest `LTS` version of Node.js is recommended.

If none or low version of Node.js is installed, you need install the latest version of Node.js according to the following instructions:

1. **For Windows**: please visit [https://nodejs.org/](https://nodejs.org/) to download the latest `LTS` version of Node.js and then, install it using the default options.
2. **For Mac**: the same as Windows.
3. **For Linux**: using package manager to install is recommended, because in this way, you don't need to configure the `PATH` variable. If you fail, you can also use the binary version of Node.js directly.
   * **using package manager**: follow the instructions [here](https://nodejs.org/en/download/package-manager/)
   * **using binary version**: visit [official Node.js website](https://nodejs.org/en/download/) to download the latest _Linux Binaries_ \(or using command `wget` to download\), unzip \(`tar -xzvf node-xxx.tar.gz`\), add the absolute path of bin directory to system `PATH` after extracting.

You can execute `node -v` in shell to check if the expected version of Node.js is installed successfully:

```text
$ node -v
v8.9.4
```

