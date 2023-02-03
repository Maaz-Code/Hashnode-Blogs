# Comms Chat Application

Hey y'all, I am back. This time with a new project of mine. ***Comms***

### Introduction

Started this open-source project not so long ago. Introducing a chat application that I was recently working on - **"Comms"**. This is a communication web application where people can have real-time conversations with each other. I have been working on ReactJS for some time and Material UI so I thought why not let's check out NextJs and a new UI framework? NextJS was something that I was using in my internship at that time. The project assigned was made using NextJS so I thought this would be an excellent chance to learn it and even apply it to a personal project. I completed this project up to a basic usage level with all the ground-level features needed.

### Tech Stack & Links

* [NextJS](https://nextjs.org/)
    
* [SCSS](https://sass-lang.com/)
    
* [Chakra UI](https://chakra-ui.com/)
    
* [Firebase](https://firebase.google.com/)
    
* [React-Firebase-Hooks](https://github.com/CSFrequency/react-firebase-hooks)
    
* [Vercel](https://vercel.com/home)
    

### Idea & Planning

I always wanted to try out NextJS as it had such great features for a developer and its regular updates. This project has enabled me to do so. My idea was to create a real-time chat application where the users would be using their Gmail accounts for authorization and identification. The communication would be possible from account to account only. So to attain this security and account system, I used my Firebase experience here. The Google OAuth provided by Firebase came in handy. Hence I created a sign-in (via Gmail) page for the app. To make the page more interesting, I further added some moving shapes animation. Built on this advance and extensive NEXT framework The page turned out like this:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1667852844347/phQU4Kg32.png align="left")

### Project Structure & Dependencies

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1675364191901/5e73c279-706c-466d-b58e-7f733d91a1b4.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1675365691498/0de279cf-5c46-4be0-98fe-e046c130d96b.png align="center")

### Working & Features

When you log in, a different UI comes up where one can chat with other people with their Gmail IDs visible on the left panel. On the left panel, there is a button to add a new chat and on clicking that, a new prompt opens up where we simply enter the Gmail addresses of the recipients. At the bottom, there is a space for typing messages and sending them. On the right side of the screen, there is a logout button. I have added the basic functionalities to understand how a chat application works. Now the working is simple as the Firebase is doing the most part via its SDKs. Firebase provided the login Oauth components via Google. Also, when we create a new chat with someone with a different ID then a new document is created in Firebase and further all the chats happening get stored in real-time into separate documents with their respective timestamps. All the activity happening from logins to chats is stored and can be monitored. React-Firebase-Hooks came in really handy while building this project to easily utilize Firestore. The UI which is built by using JS logic with Chakra UI looks like this upon sign-in.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1674504363170/d152c0be-f5f4-4403-ab0b-acd88eaa30c2.png align="center")

### Future work

* Make the application responsive and mobile-friendly so that it can be used by gadgets of different screen sizes as well.
    
* Add more sign-in options like GitHub or Twitter.
    
* Provide more things to be shared in chat like emojis or images.
    
* Names instead of account IDs should be visible to the users.
    
* Try out DevOps and Cloud lifecycles as well.
    
* Add a dark theme option for users.
    

### Conclusion

This blog was pending for a long time but now I have finally summarized this project and mentioned all details. I have kept the project in the Open-Source format with templates for anyone to contribute. I am looking forward to your suggestions and feedback. So do give it a try from the links below. I will continue updating this. Kindly subscribe to my newsletter to stay updated on my blogs. Thank You!

Live Link: [Comms](https://comms-chat.vercel.app/) | Repository: [GitHub](https://github.com/Maaz-Code/comms)