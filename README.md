Welcome to the most basic of BIG-IP Next 20.x labs. We are creating a few scenarios to show off some of the BIG-IP Next 20.x changes. 

Lab 1: The one that works (mostly). 
- Refer to the Rapidlab screenshot (lab1_rapidlab.png) to create a BIG-IP Next lab consisting of 1 Central Manager instance and 2 LTM instances.
- Once the lab is available, log into the Central Manager. Ensure your LTMs were automatically added as a high availability pair.
- Use the application import tool to import the UCS file in the lab, making use of the included masterkey as well.
- Take a look at the configuration items. Most of them imported correctly. One did not. Why not?

Lab 2: CM Clustering and LTM Discovery.
- Deploy a new Rapidlab based on the lab 2 screenshot (lab2_rapidlab.png) with 3 Central Manager instances and 2 LTM instances. Ensure the boxes to automatically script the high availabilty and discovery are unchecked per the screenshot.
- After the instances are ready, create the Central Manager cluster with 3 nodes manually.
- Then discover the two LTM instances and create a high availability pair.
- Then load the same UCS as used in Lab 1.
- Rename and Re-IP one of the virtual servers during the import process. 
- There will be some issues encountered along the way. Why?

Lab 3: Application creation via GUI (placeholder)
- configure a Rapid Lab deployment with a CM and a pair of standalone instances and one Ubuntu Server
- configure apache on ubuntu to listen on two different ports that will simulate two nodes, modify index.htm so that they have slightly different text
- Manually via GUI configure straight HTTP application
- Manually via GUI configure HTTPS off loading


Lab 4: BIG-IP Next, AS3 and YOU! (placeholder)
- Setting up an environment to post AS3
  - I used REST client inside of VSCode
    - https://docs.f5net.com/display/CONSULTING/Using+VSCode+to+send+AS3+to+BIG-IP+Next+API
- Differences between Classic TMOS and BIG-IP Next
  - no AS3 package to install (native)
  - declerations get posted to a different API point
  - know the difference between simply posting a document and an actual deployment
- Deploy application configurations to the BIG-IP Next system using AS3 decleration
  - Simple HTTP via AS3
  - Simple HTTPS via AS3
 
Lab 5: BIG-IP Next WAF Security (placeholder)
- create a security policy
- deploy a security policy
- attack your site and get some logs to view

Lab 6: BIG-IP Access
- configure and deploy an access policy for a simple HTTPS site
 
