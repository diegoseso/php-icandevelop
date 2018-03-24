# php-icandevelop
Learning the basics of php / html / css / git / docker introduction 

## Welcome

So you want to learn this web stuff ? I want to try to teach you, but for this I´d rather guide you to discover it all by yourself

First of all you need to be able to execute git program on your machine. If you do not know what is git / github I recommend you to go to 
https://try.github.io/levels/1/challenges/1

I recommend you to go to https://github.com/join and make yourself an account. 

Once you have made the tutorial and have an account I think you are ready to download this project, for this you just need to execute
the following code on the terminal

    git clone https://github.com/diegoseso/php-icandevelop.git
    
Now you have this code locally, at this point you will find a Dockerfile. Oh my god too many things to learn, what is docker ? 
I think you should read this https://www.docker.com/what-docker

If you have been curious enough I think now you know what a container is. My guess is that you want to install it to go further! 
Install docker on your machine by following https://docs.docker.com/install/

On this project that you should already have on your machine (remember you cloned it) I left setup for you this dockerfile that sets a php server only,
before making it work I think you should learn a little bit on how to use docker https://training.play-with-docker.com/dev-landing/

If you rather go to make the server work you just need to run the following code

    docker run -itd -p 8001:80 -v ${PATH_OF_THE_PROJECT}:/usr/share/nginx/html nginx

Where ${PATH_OF_THE_PROJECT} is the local route where this project is in your machine, for example if you cloned it inside your home folder in a linux machine it could be /home/myuser/php-icandevelop
if you are on a windows machine it could be something like C:\documents and settings\php-icandevelop


If everything went well now you can go to your browser an  type in the following url

    http://localhost:8001
    
What do you see ? 

If you see a message like "Welcome to nginx!" you are on the right path ! If not I suggest to check your steps 
and contact me.

Now, assuming you are on the right track what happens when you try to go to 
    
    http://localhost:8001/index.php
    
My guess is that the index.php downloaded instead of been executed , why is that ? 

## Important 

Do you think I am missing something here ? make a Pull request ! 