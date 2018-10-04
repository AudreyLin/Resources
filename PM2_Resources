                                                  **PM2 Resources **
                                                 
   [PM2.IO](https://pm2.io/)
   [PM2Runtime](https://pm2.io/runtime/)
   [PM2 Blog](https://blog.pm2.io/)
   [PM2 Pricing](https://pm2.io/pricing/) - The OpenSource Runtime Version is free.  There is an Enterprise version for $30/mth & one that you can have custom build & managed for you.  
   
   
   
   PM2 is free to use for the Runtime version.  It is basically a process manager.  It allows you application to run multiple automated processes, setup your environment, log management, integrate into your project & a number of other things I haven't expolored, yet.  I'll definitely be using it with my projects in the future.  I still have a lot to learn, but I'll write what I can as I learn more.  Right now, I have used it in CentOS in a VPS for Bluehost. 
  
  
   <strong>First I deployed my React App</strong>
                                                  
   For the project I just did with PM2, I deployed my app with a live GitRepo to my Bluehost CentOS VPS via ssh.  I used [BaseNineStudios' Playlist](https://www.youtube.com/watch?v=2q8cW9mQtOM&list=PLZuMe24DqTOJbtifcCproNbi_o1thRJs4) to learn how to do the live repo deployment. (That playlist is for Bluehost, but I think it applies to any CentOS VPS. )  
   My project was a React application that ran an Express backend.  (I had to sudo into root for some of this, but I had the access.)  
   I had to CD into the PUBLIC_HTML where I hooked the live repo & CD'd into the client folder for React & ran      
   
                                          npm run build
                                          
 then since I was running a node environment
 
                                          npm install -g serve
                                             serve -s build
                                             
You can read more about your [React Deployment Here](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/README.md#deployment) - It could be different for you.  I probably could have just used my NodeExpress backend to set it up, but I just went with the serve npm package since it was my first time & it took me forever to figure everything else out. 
                                         
<strong>Then I installed PM2 Runtime</strong> into my VPS.  
                                          
                                          npm install pm2 -g
                                          
    Then, I was still in my VPS Repo and installed the CLI autocompletion tool
    
                                          pm2 completion install
                                          
      (The autocomplete CLI tool helps to finish typing the next directory or file in the path when you start to type something and hit "tab".)  
   
   Then, to keep the pm2 up to date & to refresh the daemon (a daemon is a background process)
   
                                            npm install pm2 update
                                            
   Then, you need to setup your [Ecosystem File](https://pm2.io/doc/en/runtime/guide/ecosystem-file/) by editing the ecosystem.config.js which you can start a template with your terminal 
   
                                            pm2 init
   The rest of the instructions will be [here](https://pm2.io/doc/en/runtime/guide/ecosystem-file/) - I will post better notes on how I did the rest of that on my next project. 
   
   
   
   
   
*Side Note Below* -Prob doesn't matter, but I just put it for reference for myself. 

   I will be using it in Digital Ocean (probably Ubuntu) next time for my personal projects.  I was going to use Heroku, bc deployment is so easy, but I think the cost will be more expensive over time.  I don't plan on personally growing to such a size, but I know that if I use it for developing sites on the entreprenuerial road, it will be something to take into consideration.
   I like Heroku.  I'll be using the sandbox version for all of my non-deployed projects/hobbyprojects/tests.  I will probably consider it more when I get to that point.  Bc I think that both Heroku & Digital Ocean are fairly straight forward and easy to use.  I know that there are a lot of others, but those are what I am familiar with just now.  (I don't think I will be using Bluehost for VPS again because there is not enough documentation or support for the VPS.  I love Bluehost for shared hosting, though & the customer service is great.)
   
   
