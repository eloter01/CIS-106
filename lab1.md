# Lab 1 Exploring Linux Distributions
---
## Requirements:
* **You will use Github to submit this Lab. Watch the 'What is Git and Github?' video before your start**
* Create a Github account before your start this lab.
* Bold your answers *(2 points)*
* Format your screenshots accordingly (not too big, not too small). If I can’t read it, I cannot grade it.
* Video: https://youtu.be/8Sa52S527Qc


## Working with Distrowatch
---
### Question 1
During class, we explored the concept of Linux distribution. During this lab, you will research some Linux distributions using a website called Distrowatch. DistroWatch is a website that provides news, popularity rankings, and other general information about various Linux distributions and other Unix-like operating systems such as OpenSolaris, MINIX and BSD. 

Go to [Distrowatch](https://distrowatch.com/). Explore the website to get familiar with the home page. On the top left corner, you have a form that allows you to submit queries to the website. In the **“Type Distribution Name”** box type **“Ubuntu”.**  This will return details about Ubuntu. Explore the Ubuntu Distrowatch page and answer the following questions:

1. What is the OS Type: 
   * **Linux**

2. Which major distro is it based on?  
   * **Debian**
   
3. Which processor architecture does it support?  
   * **armhf, i686, powerpc, ppc64el, s390x, x86_64**

4. Is the distribution active or is it discontinued?  
   * **active**

5. What is the distro’s home page?  
   * **https://ubuntu.com**

### Question 2
On the top left corner, click on “Random Distribution” and answer the following questions from the distro you got.
1. What is the name of the distribution and the OS Type: 
   * **Lunar, Linux**

2. Which major distro is it based on?  
   * **Independent (forked from Sorcerer)**
   
3. Which processor architecture does it support?  
   * **i386, i686, x86_64**

4. Is the distribution active or is it discontinued?  
   * **active**

5. What is the distro’s home page?  
   * **http://www.lunar-linux.org**

### Question 3
On the top of the page, right in the middle, you will find an option that allows you to search for distributions. 
Click on **“Search”** and after the page loads, fill in the following information in the **“Search Distribution by Criteria”** section and Click on Submit Query.
* OS Type: Linux
* Architecture: x86_64
* Status: Active
* Leave the rest as default.

From the query results, choose any distribution and answer the following question about the distro you chose.

1. What is the name of the distribution? 
   * **Zevenet**
  
2. What is the country of Origin?
   * **Spain**
  
3. What major distribution is it based on?
   * **Debian (Stable)**

4. What is the distribution category?
   * **Server, Specialist**
  
5. Which processor architecture, aside from the one in the original query, does the OS support?
   * **none other**

### Question 4
Now that you know how to use Distrowatch. Find a Linux distribution for the following scenarios. For each distribution provide the website, name, and supported architecture.

1. A Linux distribution used for Data Rescue/Data recovery
* Distro Name: **Finnix**
* Website: **https://www.finnix.org**
* Desktop Environment: **No Desktop**

2. A Linux distribution used for Education that supports the ix86 processor architecture.
* Distro Name: **Karoshi**
* Website: **https://www.linuxschools.com/**
* Desktop Environment: **Xfce**

3. A Linux distribution that supports the OEM installation method
* Distro Name: **Kubuntu**
* Website: **http://www.kubuntu.org/**
* Desktop Environment: **KDE Plasma**

### Question 5 (Extra credit 2 pts - Optional)
On the Distrowatch homepage in the menu located in the middle of the page, you will find an option called **“Submit Distribution”.** This option lists all the Linux distros that are pending evaluation, on development or that are experiencing some sort of legal constraint.  Select one of these distributions and in a paragraph, share your thoughts. (keep it simple 5 to 8 sentences).

I chose a distribution called [Donau](http://www.donau-os.com/), a Debian Stretch based system which was submitted on 2019-03-27 and is under the "Projects not yet ready" section. Given the lead developer's name (Rareș Rășcanu), my guess is this is based in Romania. I checked out their latest news and the last post was on 3/26/2020 where the developer celebrates the one year anniversary of Donau by releasing the newest version of the system called Donau Lotus. The developer describes the improvements to the new version and urges users to vote for the distribution since, as distrowatch puts it, "every Tom, Dick and Harry has now created one" and the submission process can take a long time. This made me giggle because it made me think of every developer who dreams of releasing their own distribution one day. However, the developer has not posted a recent update since March 2020, also the start of a lot of national shut downs, which makes me wonder if that has something to do with it. In any case, it is still waiting to be added to the database.


## Working with DistroTest.net
### Question 6
DistroTest.net is a project that allows you to test Linux/BSD distributions on your web browser. This website is great for trying out distributions before you even download the ISO file. Go to [Distrotest.net](https://distrotest.net/) and click on any of the distributions. Start the distribution and take a screenshot of the browser window that just popped up.

![ufficioZero](ufficioZero.png)

Locate the terminal application in the distribution you started and type the following command: `uname -a` Take a screenshot of the browser window showing the terminal application open.

![xubuntuUname](xubuntuUname.png)

Stop the machine and take a screenshot of the browser window showing that the machine has been stopped.

![noVNC](noVNC.png)
