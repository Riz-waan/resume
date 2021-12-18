[<-- Home](../README.md)

## Chattanooga Islamic Outreach

![](https://img.shields.io/badge/-HTML/CSS/JS-white?logo=html5)
![](https://img.shields.io/badge/-Tailwind-white?logo=tailwindcss)
![](https://img.shields.io/badge/-Prismic_CMS-white?logo=prismic)  

Project Link - <https://www.chattio.org>

This person I knew was starting a new nonprofit and he wanted me to create a Facebook compatible logo based on his original. This resulted in the following:

![](https://i.imgur.com/xiqQemp.png)

After further discussion, he said he wanted a website to be able to do the following:
 
1. Donations - They needed to be able to accept PayPal Donations.  
2. Mailing List - People need to be able to sign up to the mailing list.
3. Statement - The mission statement should have a place.
4. Gallery - There should be a place to upload images grouped based on events/folders.
5. Events - There needs to be a page listing all of the events planned and completed. 
6. Resources - A page to post local resources such as job opennings, etc.
7. Contact - There should be a contact form that sends the submission as an email.

### Design
The first step for me was to create a design that satisfies their request. This is what we came up with:

![](https://i.imgur.com/pnLTNOB.png)

### Donations
Donations was a really easy aspect. All I needed was PayPal's hosted donation button link, and I could just redirect from one of my buttons on the site to that.

![](https://media.giphy.com/media/muRfqPqLTdH3LIFT5j/giphy.gif)

### Prayer Times
This requirement was a bit hard. The problem was that unlike I originally thought, Mawaqit did not have a usable API. Furthermore, the website that they used was blocking iFrames. However, after lots of research I found out that there was an option to make it an embeddable widget by changing the URL a bit. This allowed me to do this:

![https://i.imgur.com/MoO0npy.png](https://i.imgur.com/MoO0npy.png)

### Announcements, Gallery, Classes
These three sections were almost identical in terms of backend usage. For [Chattanooga Islamic Outreach](./cio.md) I had used [Prismic](https://prismic.io) as the headless CMS option. Unfortunately, for this project the demands could not be met with that service so I had to use another one: [Contentful](https://contentful.com)
The design for these sections are as follows:

Announcement:
![](https://i.imgur.com/rgd3vUD.png)

Gallery:
![](https://i.imgur.com/y37dAhI.png)

Classes:
![](https://i.imgur.com/qM1DQst.png)

Included images within the design provided by Syed Aoun Abbas and Neda Astani from Unsplash.

The announcement was just one post in Contentful that is directly linked. The gallery just pulls all the images uploaded to contentful with the `gallery` tag. Each class is a seperate page.

### Contact
This was rather simple. I just had to pass a third party as a the form submit tag and it worked. The service I used was called [SlapForm](https://slapform.com).