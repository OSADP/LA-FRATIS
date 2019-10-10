Application Name:
Enhancement of Cross Town Improvement Project (C-TIP) Drayage Optimization Proof of Concept Application

Version Number: 
v1.0 

Primary Functions:
Minimizing total time for execution of drayage operations
Minimizing total distance for execution of drayage operations
Traffic delay consideration when generating route solutions for travel time estimates
Notification of previous day and same day trips to a Marine Terminal Portal
Dynamic planning or re-optimization considering real-time parameters and driver location
Communication of daily plan and order status updates through the use of a Driver Mobile Application

Hardware Supported:
Intel/AMD based 64-bit processor architecture 

Installation Instructions:
There is no installer included with this package. Only Source code is provided. To access the main application open the web project.

In order to compile the dispatcher application the Routing projects must first be compiled and built in the following sequence:
1. PAI.Gis.Routing.Core
2. PAI.Gis.Routing.Engine
3. PAI.Gis.Routing.Traffic.La
4. PAI.Gis.Routing.Traffic.Tti

This only have to be done once for the first time running.

To ensure the code for the Marine Terminal Notification Portal runs, the follwing projects must be compiled in the below sequence:
1. cd .\PAI.FRATIS.SFL.Web\  
 
2. npm install -g bower
 
3. npm install -g gulp
 
4. npm install
 
5. bower install
 
6. gulp --app=fratis --gulpfile gulpfile.js

To be able to access it go to the following endpoint: Localhost/mto 


Size of Package:
5.73 MB (6,015,944 bytes)

Description of the applciation:
Background--
The Enhancement of Cross Town Improvement Project (C-TIP) Drayage Optimization Proof of Concept Application project had four areas of emphasis:
	********Intermodal Exchange (data sharing between all the parties), 
		Wireless Drayage Updating (focused on communicating drayage itineraries in real time), 
		Real-Time Traffic Monitoring (focused on providing information on congestion and traffic incidents), 
		and Dynamic Route Guidance (producing a more productive route for the freight carrier). 
Together, these four areas of focus can result in significant improvements in intermodal efficiency, including reductions in truck trips and reductions in travel times.  These benefits, in turn, will directly result in the public-sector benefits of congestion reduction an improved air quality. This project used the deliverables from previous projects as the foundation to build a more sophisticated application that will add value to improving the transportation network.


The optimization algorithm used in this project is an extension on the algorithm used in the Cross Town Improvement Project (C-TIP) Drayage Optimization Proof of Concept Application and the Freight Advance Traveler Information System (FRATIS) application. Due to the complexity of the drayage problem, the proposed optimization algorithm was developed through multiple iterations. In each iteration, the performance of the algorithm was validated and tested to ensure that the algorithm was working properly. The algorithm performance has been tested over a set of different problems ranging from well-known benchmark problems to specially customized ones.   

Release notes--The Drayage Optimizer will produce a solution set that represents the best determined sequence of stops, minimizing the total time for execution based upon Locations, Divers, Jobs, Routes, Traffic Delays, appointment times, equipment size, and marine terminal waiting times provided to the algorithm. Traffic delays can be provided by any third party external system that estimates travel times considering traffic within two locations.  
The solution is built leveraging v4.5 of the .NET Framework.  The optimization class library has a small footprint, and should run successfully on any computer capable of supporting .NET v4.5.  



Category:
Algorithm

Subcategory:
Transportation

Suggested System requirements:
Memory:
4GB of RAM minumum, 8GB of RAM recommended

Processing Power:
Any processor capable of running the Microsoft Windows 7 and higher operating system

Operating system:
Microsoft Windows Operating system supporting the .NET Framework v4.5 

Hard Drive Requirements:
50MB of Storage
Additional to that, there are no hardware requirements for the algorithm to work.


LICENSE:

    Copyright 2015 Productivity Apex Inc.
        http:www.productivityapex.com/
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http:www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.	
