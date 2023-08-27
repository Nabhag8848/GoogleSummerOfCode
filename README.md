# 🚢 Summary of Work Under GSoC 2023

![Heading](https://github.com/Nabhag8848/GoogleSummerOfCode/assets/65061890/836f66fd-8a83-4c2b-bf62-38b276ecdaa9)
```
       Experience the Power of Notion inside RocketChat Workspace and Elevate Collaboration
```

## ✨ Project Abstract 

`Integrate Notion Via RC App` prioritizes teamwork by enhancing collaboration for workspace users. Imagine having the power of two essential platforms, RocketChat and Notion, united as one, eliminating the need to switch between two platforms. Teams can Seamlessly Connect, Effortlessly Manage various Notion Workspaces, Share documents, and Even View Documents all within RocketChat. The real magic lies in Preserving your Important message inside the Notion Page, Structured within the Notion Database, ensuring vital discussions, decisions, and insights are never lost again, fostering alignment and inclusivity as everyone stays on the same page, even if they're not actively chatting. Whether it's brainstorming sessions, meeting notes, or shared links, find them all in one organized place. Plus, Create Comments on the Notion Page, view the Notion Database, and interact with relevant information.Welcome to a new era of streamlined collaboration, Where RocketChat and Notion work together seamlessly to fuel your team's success.

## 🌅 Glimpse of Project
-  These Video is recording of Rocket.Chat's Google Summer of Code Project Demo Day 2023, Where Contributors like me Showcase Amazing Projects they have been working on under Coding Period. 
  <p align = "center" > <strong>Tap to View </strong></p>
<p align="center">
       
<a href="https://www.youtube.com/watch?v=G1fZBqy5jp8">
<img src="http://img.youtube.com/vi/G1fZBqy5jp8/0.jpg">
 </a>
</p>

## 📦 Deliverables

1.  **OnInstallation Message from Marketplace:** When users install the Notion App from the RocketChat Marketplace, they receive a welcome message that introduces the features and further using guide of the integration.

2.  **Helper Message:** Users can access a helper message with usage instructions by typing `/notion help`. This message provides guidance on how to use various commands and features.

3.  **Smooth Authorization with Notion:** Users can seamlessly connect their Notion account to the RocketChat workspace using the `/notion connect` command. Similarly, they can disconnect using the `/notion disconnect` command, ensuring privacy and security.
    
4.  **Manage Multiple Notion Workspaces and Switch Between Them:** Users can manage and switch between Notion workspaces using `/notion workspace` or `/notion ws` within RocketChat. This allows teams with different projects to collaborate effectively by connecting the appropriate Notion workspace.
    
5.  **Create a Page or Record:** Users can create new Notion pages or records directly from RocketChat using the `/notion create` command. This streamlines the process of initiating new collaborative documents.
    
6.  **Create Notion Database:** Teams can create new Notion databases using the `/notion create db` command. This enables structured data storage and management within Notion for efficient collaboration.
    
7.  **Sharing Notion Page:** Users can easily share Notion pages with their teammates using the `/notion share` command. This ensures that relevant information is quickly accessible to the right people.

### 📝 **Extra Features or Features Which was Reevaluated:**
    
8.  **Comment On Page:** Teams can add comments to Notion pages directly from RocketChat using the `/notion comment` command. This feature encourages discussions and annotations within the context of the shared documents.
    
9.  **Viewing Shared Notion Page:** Users can view shared Notion pages within RocketChat, even if they don't actively participate. This ensures that important information is readily available to everyone.
    
10.  **Preserve Message in Notion Page (Optional New Page Structured within a Database:** Users can choose to preserve RocketChat messages within a Notion page, structuring it within a database or while creating new task. This feature ensures that valuable discussions, decisions, and insights are captured in the appropriate context for future reference.

11. **View Notion Table and Update Database Entries:** Teams can view Notion database tables and update entries using the `/notion view` command. This facilitates collaborative data management without leaving RocketChat.

## 📺 Demo 
### 1. OnInstallation Message from Marketplace:

Once the app is installed from the marketplace and enabled for use, users will automatically receive a helper notification in the direct room that provides simple and user-friendly instructions on how to use the integration.

### 2. Helper Message:

The "/notion help" command serves as a valuable command for users who might require a Quick Refresher. This command ensures that users can easily retrieve essential information, providing a convenient way to use App. 

### 3. Smooth Authorization with Notion: 
The smooth authorization process for accessing and manipulating Notion pages and databases within a specific workspace directly from Rocket.Chat involves OAuth2 Notion Authorization.  user can connect to workspace using `/notion connect` and When a user wishes to disconnect from a workspace, they can simply run the `/notion disconnect` command.
- The implementation of this feature have been done using backward compatible approach and not using the Apps Engine framework's due to some limitations in Notion OAuth2 handling. Notably:
    1. **Basic HTTP Authentication**: Notion recommends using Basic HTTP Authentication during the access_token request.
    However, the Apps Engine OAuth2Client may not support this functionality at present.
    2. **Credential Format**: Notion advises providing credentials in the form of `Basic CLIENTID:CLIENTSECRET` in base64 format,
    which might not be fully supported by the Apps Engine OAuth2Client.
    3. **Extra Fields**: Notion integration requires additional fields in persistence storage,
    demanding customization of the Apps Engine to accommodate these fields.
    
### 4. Manage and Switch Between Workspace: 
The `Manage and Switch Between Workspace` feature enables users to switch between previously connected workspaces without the need to fully disconnect from their current workspace. This smooth transition between different workspaces enhances productivity by eliminating interruptions in workflow and mitigates the risk of confusion and errors that may result from working in the wrong workspace.

### 5. Create a Page Or Record:

### 6. Create Notion Database:
### 7. Share Notion Page: 
### 8. Comment On Page: 
### 9. View Shared Notion Page: 
### 10. Preserve Message in Notion Page:
#### Preserve in Existing Page:
#### Preserve in New Page:
### 11. View Notion Table: 

## 🙌🏼 Mentors

I would like to express my heartfelt gratitude to [Bárbara Zanella](https://www.linkedin.com/in/barbara-zanella/) and [Samad Yar Khan](https://www.linkedin.com/in/samad-yar-khan/), my exceptional mentors throughout this project journey. Their unwavering support and guidance have been instrumental in shaping my growth. With their insightful guidance, we held two productive meetings each week, a testament to their commitment. Their encouragement to step beyond conventional boundaries has truly been transformative, pushing me to explore innovative solutions. From enhancing user-centric aspects to intricate technical implementations, their mentorship covered every aspect. In the face of diverse challenges at every juncture, their expertise helped us conquer each obstacle with determination.

![Team(1)](https://github.com/Nabhag8848/GoogleSummerOfCode/assets/65061890/e33b8b4c-598d-40e8-978a-b0ad4414a23f)

I Extend my sincere thanks to Sing Li and the community for their invaluable contributions. Their insights and alerts on project direction have been invaluable, enhancing the project's usability. The continuous feedback loop created by this collaborative effort has been pivotal in our project's evolution. Without this constant stream of input, our progress would not have been as remarkable. I am truly grateful for the guidance and support provided by both my mentors and the community, as they have been pivotal in making this journey an enriching and successful one.

## 👤 About Me

I'm Nabhag, a final-year Computer Engineering student from India, driven by a deep passion for Engineering. Beyond my academics, I'm devoted to crafting Plugins and Integrations that seamlessly connect various products, resulting in substantial impacts. I’m an active Contributor in the Rocket.Chat Apps Community, and I firmly believe in transparently sharing my learning journey and progress. This involvement has opened doors to exciting opportunities, allowing me to shape platform integrations and extensions. Every Hackathon fuels my passion for designing innovative plugins, while my broader focus extends to creating developer tools and products that enhance the overall developer experience. Embracing the world of open source empowers me to work on projects close to my heart. While my primary identity revolves around being an OpenSource Contributor, I've also had the honor of taking part in Google Summer of Code, which has added another layer of enrichment to my journey.

## 🛤️ My Journey

My journey in the world of technology has been quite a ride. It all began with me diving into C++ programming and exploring the intricacies of Data Structures and Algorithms during my degree course. Initially, programming felt like a foreign concept, but I gradually picked up the ropes. However, I soon felt a sense of monotony and decided to switch to Java when I couldn't find exciting projects within the realm of C++. As I delved into Java, I started creating small console applications, only to realize that I wasn't making much progress.

Then, a game-changer entered the scene: [WeMakeDevs](https://wemakedevs.org/) Community introduced me to the concept of **Learning in Public** and the intriguing challenge of **100DaysOfCode**. This was my gateway to the world of Full Stack Development. Embracing this approach, I began sharing my daily learning experiences on Twitter. Thankfully, through the 100DaysOfCode Challenge, I connected with like-minded individuals who shared my passion.

As I continued, I found myself gravitating towards Backend Engineering. However, I realized that I was stuck in a cycle of endlessly learning without any concrete application and missing real users. Seeking a breakthrough, I embarked on an internship with a fintech startup. Here, I was responsible for crafting an Investing Monitoring Tool that offered real-time analytics for trading Crypto using a blend of WebSockets, Angular, and NestJS. This was a pivotal moment as it marked the first time I developed something truly useful for users.

As my journey progressed, I became intrigued by the inner workings of communication protocols and the world of open-source software. My curiosity led me to participate in HacktoberFest, where I started trying to contribute to various organizations. Eventually, I stumbled upon RocketChat Apps, which opened up a new dimension of integration. This was exciting and novel, and I immersed myself in the Apps ecosystem. It was a joyous achievement when my pull request was merged into the Rocket.Chat repository, becoming a part of the Rocket.Chat 6.0 Release.

Joining Rocket.Chat came with a learning curve. Unexpectedly, my open-source journey paved the way for Google Summer of Code (GSoC). While I hadn't initially planned for it, the contribution mindset propelled me forward. I felt drawn to GSoC's mission of introducing more people to open-source, which led me to craft a proposal for Integrate Notion via RC App, just days before the deadline. It was a whirlwind of activity, including Creating a Figma design within a week. Miraculously, my proposal was accepted, bringing an indescribable sense of joy.

Transitioning into a Google Summer of Code Student was enlightening. As my mentor rightly said, getting selected is one challenge, but making the project a success requires relentless effort. The coding period had its share of ups and downs. Early on, we developed features, but they lacked a user-centered approach. The turning point arrived with valuable feedback from the community. This feedback reshaped our project into a more user-centric one, even though the challenges escalated.

The journey has been nothing short of a rollercoaster. We tackled seemingly impossible features within tight deadlines, all while dealing with Notion's limitations. This experience has been amazing and has firmly rooted me in the world of open-source. Once you dive in, there's no looking back. This is a journey I'm truly passionate about. If you're interested in venturing into open-source, feel free to connect with me on any of my social media platforms mentioned below.

## 💬 Connect With Me
<div align="center">

| **Student** | Nabhag Motivaras |
|:--------------------|:-------------------|
| **Organization** | [Rocket.Chat](https://rocket.chat/) |
| **Project** | [Integrate Notion Via RC App](https://summerofcode.withgoogle.com/programs/2023/projects/9v76k7Q8) |
| **GitHub** | [@Nabhag8848](https://github.com/Nabhag8848) |
| **LinkedIn** | [Nabhag Motivaras](https://www.linkedin.com/in/nabhag-motivaras-460b3b1aa/) |
| **Email** | <a href="mailto:nabhagmotivaras76@gmail.com">nabhagmotivaras76@gmail.com</a> |
| **Rocket.Chat** | [nabhag.motivaras](https://open.rocket.chat/direct/nabhag.motivaras) |
       
</div>



