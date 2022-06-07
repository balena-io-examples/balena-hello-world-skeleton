# balena-hello-world-skeleton

This is a skeleton repostiory to use as a template for adding support for a new language example in balena. Make sure to keep the repository structure and files as uniform as possible with other balena-hello-world examples. Process to create a new language example:

1. Create a new repository using this template. 
2. Add your language specific server's source code, assets and files
3. Build the `Dockerfile.template` and edit `.gitinore`, `.dockerignore` as needed 
4. When implementation and testing is complete, finish adding details to `balena.yml`, `repo.yml`, `README.md` and a logo for the language.
5. Push the changes to GitHub and have the repository transferred to balena-io-examples organization. 

You can create issues on this template repository to let us know of a new language example that you are building and ask questions regarding the same.

# A Simple Server with LANGUAGE

[![balena deploy button](https://www.balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/balena-io-examples/balena-LANGUAGE-hello-world)

This is a simple skeleton LANGUAGE server project that works on any of the [devices supported][devices-supported] by [balena][balena-link].

This project serves up a welcome page on port `:80` of your balena device.

To get this project up and running, you will need to [sign-up][signup-page] for a balena account. Have a look at our [Getting Started tutorial][gettingStarted-link] to help you kickstart your journey in creating a fleet of devices. Once you are set up with balena, you will need to clone or download this repository. 

After downloading, navigate to the directory and run the `balena push` command using the [balena CLI][balena-cli]. This command will package up and push the code to the balena builders, where it will be compiled, built and deployed to every device in the fleet. When it completes, you'll have a LANGUAGE powered web server running on your device and you can see some logs on your [device dashboard][balena-dashboard].

```bash
cd balena-LANGUAGE-hello-world/
balena push <FLEET_NAME>
```

To give your device a public URL, access the device page on the [balenaCloud dashboard][balena-dashboard], and choose the _Public Device URL_ toggle. Once the device is updated, check the Public Device URL to find the welcome page showing up from your device. That's it, you have deployed your first balena device!


[balena-cli]:https://www.balena.io/docs/reference/cli/
[balena-dashboard]:https://dashboard.balena-cloud.com/
[balena-link]:https://balena.io/ 
[devices-supported]:https://www.balena.io/docs/reference/hardware/devices/
[gettingStarted-link]:https://www.balena.io/docs/learn/getting-started/raspberrypi3/LANGUAGE/
[signup-page]:https://dashboard.balena-cloud.com/signup
