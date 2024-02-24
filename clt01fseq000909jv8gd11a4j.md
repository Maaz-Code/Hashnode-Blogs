---
title: "Develop and Publish your own CLI app within minutes (ClackJS + Node + NPM) 🚀"
datePublished: Sat Feb 24 2024 12:09:10 GMT+0000 (Coordinated Universal Time)
cuid: clt01fseq000909jv8gd11a4j
slug: develop-and-publish-your-own-cli-app-within-minutes-clackjs-node-npm
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1706298224740/4e616291-22bf-47e2-9053-b319730ff88f.png
tags: javascript, nodejs, projects, npm, cli, passwords

---

## Introduction

CLI (Command Line Interface) is simply a text-based interface used to interact with computer systems and software by entering commands. Instead of using a graphical user interface (GUI) with icons and buttons, users interact with the system by typing text commands into a terminal or console.

**PasswordCLI** is a CLI project made using Javascript that lets us generate unique random passwords based on the inputs we provide. It has a straightforward flow with multiple choices built from scratch with just a few lines of code.

## Tech Walkthrough

1. [**ClackJS**](https://www.clack.cc/)**:** Created by Nate Moore ([natemoo-re](https://github.com/natemoo-re)). I have used the package derived from *clack/core* commonly known as *clack/prompts.* Clack is simply a framework written in TypeScript that enables us to create enhanced and interactive CLI applications. It has different prompts that one can easily leverage into their project. It comes with beautiful components and straightforward APIs.
    
2. [**Generate-Password**](https://www.npmjs.com/package/generate-password)**:** It is a great npm library I found to implement the random password generation code. I was able to its vast variety of options for the type of functionality I would want for the users.
    
3. [**Figlet**](https://www.npmjs.com/package/figlet)**:** A FIG Driver written in JavaScript which aims to fully implement the FIGfont spec. I used this to add a unique element to the console. This helped me print a customized styled text at the end of the application. A good amount of fonts and styles are available in this package.
    
4. [**NPM**](https://www.npmjs.com/package/@npm-i-maaz/passwordcli)**:** The npm Registry is a public collection of packages of open-source code for Node.js, front-end web apps, mobile apps, etc. npm is the command line client that allows developers to install and publish those packages. Node Package Manager is the central part of the project as all the tech I used is present in the form of npm libraries. Moreover, I have used this to publish my CLI tool globally to be used on any machine anywhere.
    

## Code Walkthrough

* Initially, we can see the NPM packages we have used and imported into our project which we will be using later. I have tried to use the maximum ClackJS prompts possible for this project and other packages. All the colors used are from the package *picocolors.*
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707594297933/d33d6182-0730-4ca5-96d0-8217276e81e7.png align="center")

* Now, we will be adding the input prompts for the users. I have provided input options like the length of the password where I have kept the password should be greater than 5. I have also provided options to include numbers and symbols in your password to make it more strong. Furthermore, users can also generate multiple passwords of the same type.
    
* The cancel methods are written to handle the cases when any operation is canceled in between and the program is stopped.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707594414762/5324edb8-30a5-4415-a437-63b0359ff542.png align="center")

* Here, the code to generate passwords comes with our generate-password package's help. Taking in all the inputs that the user has given via the prompts, the function executes and generates a random unique password whether it's single or multiple.
    
* If you dig down to the source code of this library, you will find more arguments that can be used with its generator function.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707594680123/f2fd0f0f-4c76-49c3-b5c0-fad7069b56a9.png align="center")

* Lastly, there is some error handling to cover edge cases and ways to show multiple passwords. I have also made sure that the users do not mistakenly pass ***null*** values in the inputs to avoid errors in the output.
    
* The use of **Figlet** can be seen in the code to produce a cool text at the end of the output. I am just printing the name of the project with a ***Standard*** font.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707594718039/f990f012-50ca-4cc6-a112-1a894be074ef.png align="center")

* For you to use your application on any other machine instead of your local machine, you have to publish your project as I did on "**npm".** The steps are quite simple you have to log into your npm account first using your credentials. This can be done in the CLI itself using `npm login`. After successfully logging in, run `npm publish`. This will automatically publish your project as a package on npm.
    
* Make sure to update of project version before every update via **package.json** so that a new version is created. The command to run this app will be generated, which anyone can use from anywhere.
    

## Try it yourself

Alright, now you are ready to create your own interesting CLI app. And, if you want to try out mine you can simply open up your command prompt and run the command,

`npm i @npm-i-maaz/passwordcli`

Subsequently to run the program anytime later this command will also work:

`npx @npm-i-maaz/passwordcli`

Follow along with the prompts and your passwords will be generated.  
The code has been pushed to **GitHub**: [PasswordCLI Tool](https://github.com/Maaz-Code/PasswordCLI)  
⭐Star the repository for future updates.

In the end, I want to share that I got to know about this idea and was inspired to make my own project after reading a similar blog by **Jessica Wang**. So big shoutout to her, do read her other blogs.

Finally, do share your thoughts or suggestions, or doubts in the comments. Also, showcase if you build your own CLI application after this. You can follow me on [GitHub/Maaz-Code](https://github.com/Maaz-Code/PasswordCLI) or other socials for more diverse projects.  
*Thanks for reading and see you at the next one!*