[<-- Home](../README.md)

## Masjid Muhammad

![](https://img.shields.io/badge/-HTML/CSS/JS-white?logo=html5)
![](https://img.shields.io/badge/-Tailwind-white?logo=tailwindcss)
![](https://img.shields.io/badge/-Contentful_CMS-white?logo=contentful)  

Project Link - <https://www.mmuhammad.org>

It all started when I was contacted about making a website for the local downtown masjid after I had finished the project for [Chattanooga Islamic Outreach](./cio.md). They had given me a set of guidelines for what the website needed to be: 
 
1. Donations - They needed to be able to accept PayPal Donations.  
2. Prayer Times - The prayer times of the mosque needed to be accessed and linked to Mawaqit (a service they were using).
3. Announcements - It should be easy to quickly add and change the announcement at the website.
4. Gallery - There should be a place to upload images with captions.
5. Classes - There needs to be a section to list the different classes offered.
6. Contact - There should be a contact form that sends the submission as an email.

### Design
The first step for me was to create a design that satisfies their request. This is what we came up with:

![](https://i.imgur.com/pnLTNOB.png)

### Donations
Donations was a really easy aspect. All I needed was PayPal's hosted donation button link, and I could just redirect from one of my buttons on the site to that.

![](https://media.giphy.com/media/muRfqPqLTdH3LIFT5j/giphy.gif)

### Prayer Times
This requirement was a bit hard. The problem was that unlike I originally thought, Mawaqit did not have a usable API. Furthermore, the website that they used was blocking iFrames. However, after lots of research I found out that there was an option to make it an embeddable widget by changing the URL a bit. This allowed me to do this:

![https://i.imgur.com/MoO0npy.png](https://i.imgur.com/MoO0npy.png)

### Announcements