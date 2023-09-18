# osTicket-Post-Install-Configuration


<h2>Technologies</h2> <!---think about how well this tracks in ATS for resume, also think about making it all encompassing--->

-  Windows 10
-  Internet Information Services (IIS)
-  HeidiSQL
-  mySQL


<h2>Prerequrisities</h2>

-  <b><a href="https://github.com/narvee09/osTicket-installation">osTicket</a></b>
-  <b><a href="https://github.com/narvee09/Client-Creation-VM-">Virtual Machine Lab Environment</a></b>


<h2>Role Configuration:</h2>
Navigate to the admin panel > agents > roles > add new role > input “Supreme Admin” > check all permissions

<h2>Department Configuration:</h2>
Navigate to the admin panel > agents > departments > select add new department > input name system administrators > leave all default settings > create department

<h2>Configure Teams:</h2>
Navigate to admin panel > agents > teams > select > add new team > input “level 2 support” > under the members tab add yourself to the team

<h2>Allow anyone to create tickets:</h2>
Navigate to admin panel > settings > users > settings > uncheck require registration and loign to create tickets

<h2>Configure Agents:</h2>
Navigate to admin panel > agents > add new agent > input [any name] with an email of [ ]@osticket.com > click set password and uncheck “send password reset email” and uncheck “require password change at next login” > set > add this person to system administrators 
Create a new agent [any name] > set department as support > view only 

<h2>Configure Users:</h2>
Navigate to the agent panel > users > create new user > input [any name ] with email @osticket.com > add user > create more users 
(this might be a good place to showcase user generation with powershell)

<h2>Configure SLAs:	Service level agreement</h2> <!---(time admin expects tickets to be resolved)--->
Navigate to the admin panel > manage > SLA > add new SLA plan > input name “SEV A” and set the period to 1 hours and schedule of 24/7
Add new SLA plan > input name “SEV B” set the period to 4 hours, schedule 24/7
Add new SLA plan > input name “SEV C” set the period to 8 hours, schedule M-F

<h2>Configure Help Topics:</h2>
 Navigate to the admin panel > manage > help topics > add new help topic 
Create the following:
Business Critical outage
Personal Computer Issues
Equipment Request 
Password Reset
