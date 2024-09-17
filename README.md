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
