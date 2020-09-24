---
title: Setting up Fider
date: 2020-09-24 23:07:00 Z
---

For this week's blog entry I am discussing how I set up fider https://getfider.com/.  Fider is a fantastic, super simple tool to help involve users in software development.  It allows people to post an idea and it can be up voted by other users.

Initially, when I went onto the site x. I was able to follow the instructions to easily set it up on a free instance with heroku.  This was a service I hadn't used before.  https://www.heroku.com/

Heroku allowed me to set up a postgres database easily and pull the code from github.  There were just a few settings to add to get the app running and it was automatically secured.  What was great is that I could have paid just $7 a month to have them host it and everything was easy.

I then got a bit more adventurous and looked to set it up on docker with Hetzner Cloud https://www.hetzner.com/.  I am not hugely experience with docker but I used two tutorials to help with it;

1. https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04 < I only did step one
2. I then edited the config file from the fider website and just put in the email server details.  I like sendinblue which offers a free smtp relay. 
3. I tried to run the command, docker-compose pull - but it turned out I needed to install docker-compose first.
4. I then ran docker-compose pull - which set up the app
5. docker-compose up - got the app running.
6. I entered http//mydomain.com:9999 in my browser and was quickly taken to the setup page.
7. Just added my email address, verified and was in the web interface changing settings.

I found the ssl settings difficult.  So instead I decided to use cloudflare to secure the connection.  Sensitive data was not being entered, but ssl is a must these days.

To really secure this properly I need to work out how to mount a volume in docker and add the two settings in the fider config.

I wanted to share as it's a fantastic app that will be useful to others.  It was a bit of a learning curve.  But I found it very interesting and got me onto other things I wanted to learn.