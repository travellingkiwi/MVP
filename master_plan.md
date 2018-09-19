Initial version written by @leonardobdes.  
If you add text, please identify your lines with @username. 

# Goal
Create a single system that comes preinstalled with multiple tools that helps work with F5 devices.

# Code of Conduct
Please do not make fun of Patrik, he is just a kid and can be traumatized.

# Project Leadership
This is a controlled anarchy, we decide based in technical reasons and not personal preference.  
Just because I am writing this does not mean I am a benevolent dictator for life (BDFL) for this project.

# Main Idea
A Linux virtual machine/container with all useful tools we use with F5 devices.  
The system should come with some base software, like iControl SOAP and REST, and other packages useful for the programs that will run on top of that, or for development and tests.  
Individual application/project will still be managed by its respective owner, but the application will come preinstalled and configured, so ready to use.

# Technical Decision – System Type
Virtual Machine, container, rpm/deb package, etc…  
I think virtual machine makes more sense in this case, as we want to install multiple packages and run multiple applications.  
Containers typically would be something disposable and easy to create and delete, limited to one application.  
rpm/deb packages, would makes things too complicate, as we would need to package different software and configuration.  

# Technical Decision – Operating System
CentOS, Ubuntu, etc..  
CentOS is what F5s uses so would be using same system as F5.  
Ubuntu is very user-friendly, has PPA, and normally has more package support.  
We could go either way here, in my opinion.  

# Technical Decision – GUI
I think we should have a small and light version, we should not have GUI.

# Tasks
We can have multiple people doing the same task, just choose what you would like to do.

* Github Maintenance  
Create readme and maintain site.  
@leonardobdes

*	System Base Setup  
Create system and share with everyone
@travellingkiwi 

*	Languages  
Install iControl and other languages

*	BigIP Report  
Find a way to have BIGIP Report in this system

*	BIG-IP Backup  
Create separated project, with a script/code that can be used to backup F5 devices configuration, or find a software that do the job.  
@leonardobdes

*	Find Tools  
Find useful tools that could be used in this system, and test  

*	Beta Test  
Test the system and report problems

*	Manual  
Create a user manual

# Github Branches
Master is the stable version.  
Beta is the test version.  
New code goes to beta, after been tested, go to master.  
