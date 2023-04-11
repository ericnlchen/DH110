# **Assignment 1: Heuristic Evaluation**
Eric Chen | DH110 | Spring 2023

## **About the Project:**
This quarter, DH110 students are challenged to design a mobile app to help family members connect with one another. The connections enabled by the app should span at least 3 generations. I aim to design a **shared family journal** to solve this challenge. For more information on my project, check out the `README.md` file at the root of this DH110 repository. For this assignment, I will be evaluating two other apps which seek to enhance family connection. I will learn their strengths and weaknesses, thereby informing the development of my own project. The framework that will be used for evaluation is described below.
<br>

## **Nielson's 10 Usability Heuristics:**
Usability consultant and human-computer interaction researcher Jakob Nielsen developed a **usability framework** composed of 10 heuristics. These general rules can be used to evaluate how effective, efficient, and enjoyable it is to use a software or technology. Here are his 10 heuristics:

| Number | Heuristic | Do | Don't
|---|---|---|---|
| 1 | Visibility of System Status | communicate state of the system to the user frequently and openly | take actions without informing the user |
| 2 | Match Between System and Real World | use common terminology, follow real-world conventions | use unintuitive jargon |
| 3 | User Control and Freedom | allow users to back out of actions by providing clearly labeled cancel buttons | trap users into actions they took by mistake |
| 4 | Consistency and Standards | adapt industry conventions to make your product similar to others like it | stray from the user's expectation |
| 5 | Error Prevention | prevent errors using warnings and effective default options | allow important decisions without user confirmation |
| 6 | Recognition Rather Than Recall | make information readily visible to reduce memory load | force users to memorize information |
| 7 | Flexibility and Efficiency of Use | allow various methods to complete actions with personalization for individual users | provide only one way to do each action |
| 8 | Aesthetic and Minimalist Design | tailor content and design to focus on a few essential elements | include irrelevant information, make the interface hard on the eyes |
| 9 | Help Users Recognize, Diagnose, and Recover From Errors | report errors in plain language, suggest solutions, use visual cues to highlight errors | use error codes or technical jargon |
| 10 | Help and Documentation | provide concise and concrete documentation as needed | overburden the user with confusing documentation |

Now we will examine two apps in detail using these heuristics as our framework!  
<br>

# **App 1: FamilyWall [(website link)](https://www.familywall.com/en/index.html)**

## **First Look:**

<p align="center">
  <img src="../Images/familywall-dashboard1.PNG" alt="Family wall main dashboard" width = "300px"/>
  <img src="../Images/familywall-explore-page.PNG" alt="Family wall start screen showing their logo" width = "300px"/>
</p>

FamilyWall is an app that seeks to connect families by providing them with acccess to shared to-do lists, calendars, photo albums, and recipe books, while also enabling location tracking and private messaging within the family group. They also offer "premium" services including budgeting and a meal planner. 

Above, you can see the two main pages of the app (which I downloaded on my iPhone for testing).
- The left image shows the *homescreen* which contains icons for the various family services (calendar, to-do list, etc). You can think of it like the iPhone homescreen which contains apps. The top menu that says "Chen" indicates which *circle* I am currently a part of. A circle is like a family group.  
- The right image shows the *explore* page, which is a comprehensive list of all available tools within the app. You can add or remove these from your *homescreen*.  

My first impression of the app is that it is generally well designed and aesthetically appealing. However, I can already foresee some usability issues. For example, the *homescreen* and *explore* page seems redundant to me. Let's dive into an in-depth evaluation of each criterion.

## **Heuristic Evaluation:**
### 1. Visibility of System Status
In my testing I immediately discovered a visibility issue. The *homescreen* is designed to allow users to access their frequently used services efficiently. They can pin or unpin services from their *homescreen*. However, the user can also unpin services from the *homescreen* by interacting with the icons on the *explore* page. When they do so, the only visual change that occurs is a small plus sign that appears next to the icon for the service which was removed. So when users unpin services in this way, it isn't clear how their action affected the state of the homepage.  

<p align="center">
  The user unpins the <em>Lists</em> service from the <em>homescreen</em> via the <em>explore</em> page:
</p>
<p align="center">
  <img src="../Images/familywall-unpin.PNG" alt="User unpins Lists service via explore page" width="200px"/>
</p>
<br>
<p align="center">
  Tiny plus sign is not sufficient communication to communicate the effect of the user's action:
</p>
<p align="center">
  <img src="../Images/familywall-small-plus.PNG" alt="Explore page is unchanged except for a small plus sign on the Lists icon" width="200px"/>
</p>
<br>
<p align="center">
  User has to navigate to <em>homescreen</em> to see the effect of their action (<em>Lists</em> is gone):
</p>
<p align="center">
  <img src="../Images/familywall-home-without-list.PNG" alt="Home page missing the Lists service" width="200px"/>
</p>

Furthermore, once the user navigates back to the *homescreen*, their unpinned services are nowhere to be seen. In order to see the services they unpinned, the user needs to navigate back to the *explore* page again, which is unintuitive.  

These issues are clear violations of heuristic 1, since the state of pinned and unpinned services is nearly invisible to the user.  

This doesn't make the app unusable but it is certainly more than a cosmetic issue. The main 2 pages of the app could definitely be redesigned to improve transparency and visual communication.  

`Severity Rating: 2`  
### 2. Match Between System and Real World
My main critique within this heuristic is the use of the word *circle* to refer to family groups. It is not immediately clear what this word means. This might not be a huge issue, except that users are confronted with this term with no explanation when they start the app for the first time. This is the screen users are presented with when they start:

<p align="center">
  <img src="../Images/familywall-new-circle.PNG" alt="Confusing startup page with word circle" width="200px"/>
</p>

This issue could be resolved by using a different term like "family group," or by providing a concise explanation of what a *circle* is when the user first starts the app.  

`Severity Rating: 1`  
### 3. User Control & Freedom
I didn't find any issues with user control and freedom. Here is a strong point I noticed with regard to this heuristic:
<p align="center">
  Each service has the <em>homescreen</em> icon at the top left to easily exit at any time:
</p>
<p align="center">
  <img src="../Images/familywall-recipe.PNG" alt="Recipe service with homescreen icon at top left" width="200px"/>
</p>

`Severity Rating: N/A`  
### 4. Consistency & Standards
This app exhibits good internal consistency, with terminology and actions remaining constant within the app.  

However, this app's external consistency is questionable. As the user, the look and feel of the *homescreen* and *explore* page remind me strongly of the iPhone homescreen, and the various family services are just like iOS apps. This analogy establishes the need for external consistency, since users will expect to be able to interact with these interfaces the same way that they interact with their iPhone homescreen. However, the consistency is not always there. For example, the *explore* page looks just like the iPhone homescreen, while the actual *homescreen* trades iOS style icons for wider icons. This makes it unclear which screen is meant to function as the user's home. Furthermore, the iPhone-esque look makes me instinctively try to swipe to switch between the two screens, but swiping isn't supported.  
<p align="center">
  Would you expect to find these icons on a <em>homescreen</em>?
</p>
<p align="center">
  <img src="../Images/familywall-explore-icon.jpg" alt="Square-shaped app icon" width="150px"/>
</p>
<br>
<p align="center">
  In FamilyWall, those icons reside elsewhere, while these long rectangular icons populate the homescreen instead:
</p>
<p align="center">
  <img src="../Images/familywall-homescreen-icon.jpg" alt="Long rectangular icon" width="200px"/>
</p>

While users can probably get used to these inconsistencies as they use the app, usability could be greatly improved by enabling iOS-style homescreen interactions wherever visual similarities to iOS exist.

`Severity Rating: 2`  
### 5. Error Prevention
FamilyWall performed well on this heuristic. One good example of error prevention that I found was the warning that is provided when the user tries to log out of their account:
<p align="center">
  Helpful warning when user attempts to log out:
</p>
<p align="center">
  <img src="../Images/familywall-homescreen-icon.jpg" alt="Logout warning" width="200px"/>
</p>

### **Top 3 Proposed Changes**

# **App 2: Chatbooks**
### **Top 3 Proposed Changes**
## **References:**
Credit given to Emily Dong for markdown syntax reference
