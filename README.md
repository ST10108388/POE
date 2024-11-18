# PROG7312_POE_PART_1 Manual


---
# DO NOT FORGET BIBLIOGRAPHY IN README
### Table of Contents

- [Description](#description)
- [How To Use](#how-to-use)
- [License](#license)
---


## Description
This is an application that seeks to improve citizen engagement and service delivery through the implementation of a comprehensive municipal services application. 
This application allows users to report issues, request services, access information about local events and announcements, and lastly receive updates on the status of their service requests.
Though this version the application the only function that works is the "Report issues and request services".

#### Technologies

- Microsoft Visual Studio 2022


[Back To The Top](#read-me-template)

---

## How To go to each window
- When the application starts up the user will be presented with four buttons that each contain writing.
- The first button is the "Report issues" button, when clicked the user will be taken to the report Issues window.
- The second button is the "Local Events and Announcements" Button when clicked the user will be displayed with an error that says that the Local events and announcemnets page is unavailable.
- The third button is the "Service Requests" Button when clicked the user will be displayed with an error that says that the Service Requests page is unavailable.
- The fourth button is the "Send Feedback" button when clicked the user will be taken to the feedback window where they are able to enter their own feedback.
  
### How to add a Report
- When the user clicks the Reprot Issues button they are taken to the report issues window
- At this window the user must select the category of the issue, then enter the name of the issue, then the Location of the issue, and lastly the description
- To add an image or document to the report the user must click the upload image button
- once the add image or document button is clicked the user will be displayed with a screen a pop up screen that allows the users to select the file they wish to upload.
- Once the user has added all of the releveant information to the report they must click the save report button.
- once the save report button has been clicked the report will be saved and displayed in the table below the description textbox.
- The user has to enter every detail before saving the report.
- If the user has not entered every detail before saving the report they will be displayed with an error that says not all details have been entered.
- If the user wishes to go back to the menu they must click the Back to menu button
- If the user wishes to dsiplay the report they must click on the Display Report Button under the save report button.

### How to Display a Report
- Once the user has clicked the display report button they will be taken to the Display Report Window.
- To display a report the user must click on the report number in the table.
- Once the report number has been clicked the user will see all the textboxes fill with data from that report they will also be shown the image or document they saved with the report.
- To go back to the main menu the user must click the Back to menu button and this will take them to the main menu.
- if the user wants to go back to the add report window the user must click the Back to report button and this will take them to the add report window.

### How to send feedback
- To send feedback the user must click the send feedback button on the main menu.
- Once clicked the user will be taken to the send feedback window.
- The user must then select the overall expereicne they received when getting the service.
- The overall experience rating is from a 1 to 5, 1 being the worst service experience and 5 being the best service experience.
- the user must then enter any suggested improvements
- the user must then enter in any comment they have.
- Once all the boxes have been filled the user must then click the Submit feedback button
- if the user has not entered in all of the details the user will then be displayed with an error saying that not all of he details have been filled in.
- if the user wants to go back to the main menu they must lcick the Back to menu button.

### How to Add a announcement or event
- Click on the Local Events and Announcement button in the main menu
- After clicking the Local Events and Announcement button you will be taken to the Display Local Events and Announcements Screen
- from this screen click on the Add event or announcement button
- After clicking this button you will be taken to the add announcemnt or event screen
- from here you must enter in all the required details
- If you miss any of the details you will be displayed with an error
- if you wish to undo the event you just added you are able to click the delete event button and this will delete your event
- once you have saved all of the event you wish to add you are able to click on the  Back to display events button and this will take you to the Display events and announcements screen

### How to display an event or announcement
- First you must select the date
- Then you are able to either enter the name of the event or announcement or select a category 
- If you type in the name of the event or announcement you will be displayed with that specific event and all of the events with a similiar category will be displayed in the Recommenedd events box
- if you select the category you will be displayed with all of the events and announcements that occured on that date
- YOu are able to click the events in the Recommended events box and you will be displayed with all of the details about the event or announcement
- to display the event or announcement YOU MUST SELECT A DATE IN THE DATE PICKER.

### How to display service requests
- To display service requests the user must click on the service requests button on the main screen
- Once the button is clicked the user will be taken to the Service request management screen where they will be displayed with four blocks
- The first block is a table that shows all of the service requests and these service requests ARE ORDERED FROM HIGHEST PRIORITY AND ALSO WITH THE HIGHEST AMOUNT OF DEPENDENCIES
- an example would be if the Service request has a priority of 1 which is the highest priority and also three dependecies it will be the first service displayed in the table
- The priorities are as follows, 1 is the highest priority and the higher the number is the lower the priority of the service is.
- In the table the user is able to view the ID of the service request to track their service request.
- the user is also able to view the status,description, estimated time that the service would take to be completed, the location of the service, the workers assigned to the service, and lastly the Date the service was requested
- If a user wants to see which services depend on each other they must click on service request in the table and they will be displayed with all of the services that are dependent on each other in the square with the heading of "Services Dependent on Each Other"
- If a service request is clicked in the table they will be shown all the details of that request in the block that has the Heading of "Selected Service Request"
- In the last block the user will be displayed with the most urgent service request. This service request has the highest priority as well as the most dependencies connected to it.
- If the user wishes to go back to the main screen they are able to click on the Back To Menu button at the bottem of the window.
- The status's go as follows, in progress means that the municipality is currently working on that service request, if the status is pending it means that the municipality has not attended to that service request, and lastly if the status is completed it means that the service request has been fulfilled.

  ## Data structures used
  ### Binary Search Tree
  #### What is a Binary Search Tree?
  - A binary search tree is a data structure that is used for organizing and storing data in a sorted manner. In a binary search tree each node in the tree has a two children, one of the children is a left child and the 
   other child is right child as stated by  (GeekForGeeks, 2024). The left child contains values less than the parent node while the right child contains values that are greater than the parent node (GeekForGeeks, 2024). 
  The benefits of using this type of hierarchical structure are efficient searching, insertion, and lastly deletion operations on the data stored in the tree (GeekForGeeks, 2024).
  #### How it was implemented
  - The binary search tree in the Service Request section of this application was used to organize and retrieve ServiceRequestModel instances based on the priority of the service request.
  - The binary search tree stores the ServiceRequestModel objects as nodes in the tree and the nodes are  arranged by the priority property. When a new service request is added it is then inserted into the Binary search tree with the following code “bst.Insert(request)” and this occurs in the method called AddServiceRequest in the ServiceRequestViewModel. To retrieve sorted service requests I used a method that was called “GetRequestsByPriority” and this method performed a in-order traversal with the following code “bst.InOrderTraversal()” In an in-order traversal of a binary search tree it returns the nodes in ascending order and therefore provided a list of ServiceRequestModel objects ordered by priority as the priority was made that so the higher the number the lower the priority of the service request is.
  - After the service request’s where retrieved in highest priority to lowest priority the list is then ordered by the number of dependencies  with the following code “OrderByDescending(r=> request.Graph.GetDependencies(r).Count()” and this prioritized requests with more dependencies. The final sorted list is returned to the SortedRequests property which is a generic list with the parameters of ServiceRequestModel and then this list is displayed in the table that displays all of the service requests in the service requests window of the application.
  - The binary search tree organizes all requests by priority and then a separate MinHeap is used to directly access the most urgent service request with the lowest priority value. The MostUrgentRequest property holds the top-priority service request.
  - The ServiceRequestsModel also checks if the tree is empty before attempting to retrieve sorted requests.
 #### How it made the application effecient
 - The Binary search tree quickly sorts service requests by priority, the Binary search tree achieves this by having each service request automatically palced in order when being inserted into the Binary search tree. This therefore saving time on sorting. The time it takes to add service requests sort them and retrieve them are 0(log n)this speed was calculated by using ChatGPT.
 - The binary search tree retrieves each service request in order of priority. This is achieved by using a in-order traversal which gets all requests in ascending priortiy and this helps to display tasks quickly.
   the speed at which it does this is 0(n) this speed was calculated by using ChatGPT.
 - The Binary search tree is able to handle large datasets well this ensures as the app can scale smoothly as more service requests are added.

   ### Graph
   #### What is a graph?
   - A graph data structure is a non-linear data structure that consists of nodes and edges as stated by (W3Schools, 2024). A point in the graph is called a node and to connect two nodes with each other a edge is used (W3Schools, 2024). Graph data structures are used in computer science to represent relationships between objects (W3Schools, 2024).
   #### How it was implemented
   - In the service request section of the application a graph structure was used to represent the dependencies between service requests.
   - Each ServiceRequestModel has dependencies represented by a list of other requests. Each of the dependencies are represented as directed edges in the graph this is achieved by the AddEdge method and this method establishes a relationship between two service requests. An example of how this is achieved is “requestGraph.addEdge(request 1, request ,1)” this code means that request1 depends on request2.
   - Each service request is added as a node in the graph using the following code “requestGraph.AddNode(request)”. Dependencies between requests are represented as edges, where the weight in this case is represented by an integer of either 1 or 2, and this weight indicates the relative importance, duration, or difficulty of the dependency.
   - The “GetDependencies” method is used to retrieve all service requests that a specific service request depends on. The “GetDependencies” method allows the “SelectedRequestDependencies” property to provide a list of dependencies for a selected request. This list of dependencies is displayed in the block with the heading of “ServicesDependentOnEachOther”. By displaying a service requests dependencies it helps understand what service requests must be completed before a specific service request can be completed.
   - In the ”GetRequestsByPriority”  method the graph data structure is used here to determine depencency counts for each request.
   #### How it made the application effecient
   - The graph data structure captures dependencies between service requests and this therefore means that related service requests are processed in the correct order and therefore reducing delays.
   - The graph allows for efficient prioritization due to nodes and edge representing service requests and dependencies. With the use of the graph the application is able to quickly find service requests with the highest urgency or service requests that depend on each other and this therefore optimizes scheduling of service requests.
     ### Heap
     #### What is a heap?
     - A heap is a complete binary tree data structure. For every node in the heap data structure the value of its children is greater than or equal to its own value (GeekForGeeks, 2024). Priority queues are implemented by using Heaps (GeekForGeeks, 2024).
     #### How it was implemented
     - In the service requests section of the application the heap is used to manage service requests and extract the service request with the highest priority which is the service request with the minimum priority value.
     -  Inside the “LoadServiceRequests” method each service request is added to the heap using the following code “heap.Insert(request)” . By doing this it ensures that the service requests are organized within the heap according to their priority.
     -  The “MostUrgentRequest” property is set to the service priority with the highest priority this is achieved by calling the “heap.ExtractMin()” method this is the code “MostUrgentRequest = heap.ExtractMin()”. The “ExtractMin()” method removes and returns the service request with the hight priority.
    #### How it made the application effecient
   - A Heap is able to retrieve the highest-priority request quickly. The Heap is also able to Add or remove service requests quickly instead of sorting or scanning the entire list.
     ### Minimum Spanning Tree
     #### What is a minumum spanning tree?
     - The definition of a spanning tree is a spanning tree that has the minimum weight among all the possible spanning trees (GeekForGeeks, 2024).
     #### How it was implemented
     - The Minimum spanning tree is being computed using Prims Algorithm. Prims Algorithm is used to find the subset of edges that connects all the nodes which are the service requests in the graph with the possible total edge weight, and without forming any cycles.
     - Prims algorithm picks the smallest edge which is the lowest weight  that connects a mew service request to the already visited ones. It performs this step by step to ensure no cycles are formed during the process. Once the edge is chosen its added to the Minimum spanning tree, and then the connected services are checked for more edges to explore.
    #### How it made the application more effecient
   - Using a minimum spanning tree ensures that service requests are connected with the least cost and this therefore avoids unnecessary connections. Prims algorithm handles large networks efficiently by focusing only on the essential connections. A minimum spanning tree saves resources and improves performance by preventing the recalculation of the same edges.
---  
   ## Project Completion Report
   - In the beginning of the semester I was extremely excited to start this project as I really wanted to implement the complex data structures we learned throughout the semester into a functional application. I learned a lot about user engagement during part 1 of the POE as before we started this POE I was not educated on the crucial ways to increase user engagement in an application and by researching five different user engagement strategies it really opened my mind to user engagement within an desktop application. I faced no challenges during part one of the POE regarding the data structures and the type of application we had to make as I already had experience with the data structures we were asked to use and also had experience with Model View View Model architecture pattern that I had to use for my Windows presentation form application. The section I struggled a slight bit in part one of the POE was making the application responsive as I only have experience with making Web applications responsive with boot strap, So having to teach myself how to make my WPF application responsive did take some time but by struggling with this and not asking for any help from any lecturers really helped me improve my problem solving skills as well as my researching skills. A section of part one of the POE where I really struggled was the uploading of different types of document and displaying them in my application. After hours of struggling I was able to get this function of the application working  and by struggling with this issue for hours it taught me how to work with different document types.
   - I really enjoyed part two of the POE as we were asked to use data structures that we have never been asked to use in a application before. I faced many challenges due to having to use data structures that I have never used in an application so having to teach myself these new data structures as well as implementing them into our application taught me how important it is to constantly be educating yourself on different data structures. A mistake that I made during part two of the POE is that I tried to add a functionality that allowed the user to be able to add their own events and announcements and by doing this it caused my application to have many issues and bugs. Another issue I had is that I over complicated the recommendation function and this also caused me to lose marks. I Believe for part two of the POE that you should used a Database as it would make the implementation of a recommendation system a lot easier as well as making the recommendation system actually a recommendation system. So in part 3 of the POE I completely removed the ability for users to be able to add their own events and announcements. A lesson I learned from part two of the POE is to mange my time better and to also not over complicate features that need to be added to applications.
 - Part three of the POE was my favourite part of this project as we had to implement complex data structures such as Binary search tree’s, Graphs, Heaps, and Minimum spanning tree’s. I really enjoyed having to learn about these complex data structures and how much faster they are compared to other data structures and how using these data structures will greatly increase the efficiency of applications. The obvious challenge I faced was that I did not have the experience with the implementation of these data structures, so I had to research how to implement these data structures and how each of these data structures functioned and how they would increase the efficiency of my application. By spending time researching these data structures it really helped me understand how to implement them into my application.
 - I have learned many new skills as well as having learnt a lot about myself from completing this POE. The major thing I struggled with in this application is the designing of the frontend as being creative is not my strongest skill but I did really enjoy implementing the backend for the application as that is where I am the strongest. In summary this POE has taught me a lot and also helped me improve as a software engineer and as a person.
---
## Technology Recommendations
- One of the best tools I believe that should be implemented into this application is a Database. By adding a database you will have centralized place to store data and therefore it makes it easier to access and manage data that is connected to the municipality application. Also using a database will allow the application to have different roles such as customer, employee, manager, and Admin. By doing this you will be able to have the creation of user accounts and this will allow for the implementation of role access control as well as allow for customers to have their own personal account and will allow for all service requests and reports to be connected to their account and also allow for the addition of a payment portal.
- A tool that can be implemented is Unit Testing as this will allow for the testing of each individual method that is in the View Models and by doing this it will ensure that each component is functionally correctly and this in turn will help reduce any errors that might occur when users a using the application.
- A great addition to this application would be the integration of a payment gateway as this would allow customers to be able to pay for services provided and if the municipality wants to expand the application to more than just services they could also allow customers to pay fines. I believe the addition of this to the application will greatly increase customer experience as customers will not have to pay for the services in person but rather online if the service they have requested is personal and not related to any government issues an example of a government issue would be potholes. To implement this payment gateway I will have to use the PayPal REST API so that I am able to integrate various payment functionalities.
- Another technology that could be implemented is SignalR . SignalR is a library for .NET that allows software developers to be able to add real-time functionality to their applications (Valdez, 2012). Real-time functionality means that server side code is able to be pushed to the connected clients as it happens in real time (Valdez, 2012). I believe this will greatly increase the quality of the application as users will be able have live tracking of the service requests, instant notification’s for local events and announcements that may be happening in the users area as well as notifications for any issues that may occur in the users area.
- The last technology that I believe should be added to the application to improve the quality of it is a CI/CD pipeline. CI/CD pipelines are automated workflows that help build, test, and deliver software quickly and efficiently (Bigelow, 2024). There are many benefits to using a CI/CD Pipeline for this application they are as follows: time is saved and human errors are reduced due to the CI/CD pipeline automatically building and packaging the application when changes are made (Bigelow, 2024). Using a CI/CD pipeline will also ensure that each release of a new feature has gone through automated testing and lastly it allows for us developers to be able to revert to a previous version of the application if the newly released version of the application has major issues (Bigelow, 2024). This Technology will greatly improve the efficiency, quality and speed of the development and this ensures that the user receives the best possible application.

## References 

References
Bigelow, S. J., 2024. CI/CD pipelines explained: Everything you need to know. [Online] 
Available at: https://www.techtarget.com/searchsoftwarequality/CI-CD-pipelines-explained-Everything-you-need-to-know
[Accessed 17 November 2024].
GeekForGeeks, 2024. Binary Search Tree. [Online] 
Available at: https://www.geeksforgeeks.org/binary-search-tree-data-structure/
[Accessed 17 November 2024].
GeekForGeeks, 2024. Heap Data Structure. [Online] 
Available at: https://www.geeksforgeeks.org/heap-data-structure/
[Accessed 17 November 2024].
GeekForGeeks, 2024. What is Minimum Spanning Tree (MST). [Online] 
Available at: https://www.geeksforgeeks.org/what-is-minimum-spanning-tree-mst/
[Accessed 18 November 2024].
Valdez, G. A., 2012. SignalR: Building real time web applications. [Online] 
Available at: https://devblogs.microsoft.com/dotnet/signalr-building-real-time-web-applications/
[Accessed 17 November 2024].
W3Schools, 2024. DSA Graphs. [Online] 
Available at: https://www.w3schools.com/dsa/dsa_theory_graphs.php
[Accessed 17 November 2024].



   

   



   
  
  




[Back To The Top](#read-me-template)

---

## License

MIT License

Copyright (c) [2017] [James Q Quick]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[Back To The Top](#read-me-template)

---



[Back To The Top](#read-me-template)
