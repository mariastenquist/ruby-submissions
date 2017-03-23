## Sinatra versus Rails Exploration

### Setup:

First, clone down the Rails project:

```terminal
git clone https://github.com/turingschool/job-tracker.git rails_project
```

And then clone down the Sinatra project:

```terminal
git clone https://github.com/turingschool/bike-share.git sinatra_project
```
Now cd into each project, run `bundle` on each project, and you're ready to go. We will only be looking at the code base and not interacting with the app. If you wanted to run the server and interact with the app, you would need to create your database, migrate your migrations, etc.

### Exercise:

1. Take a look at this stripped down Sinatra app and this stripped down Rails app. How are they different and how are they similar? Identify 5 differences, and for each one describe 1-2 implications. What effect does that difference have for each framework? If you don't know exactly, draw on your knowledge and experience and make some educated guesses/inferences. Also, practice your research skills to look into the differences.  The root of both apps is pretty similar in terms of a Gemfile, Rakefile, configuration, and the app folder both have the MVC structure in place. The rails structure is longer and more comprehensive. The rails app also has an MVC structure in it's app folder, but also helpers, assets, and mailers. Sinatra is a more lightweight framework that is good for quickly drawing up an application, whereas Rails is a better option for fully-flushed out applications and a user-generated experience. Sinatra is good for micro sites or a feature of a bigger site, where most agree that Rails is better for bigger-scale projects. If an app has 5-10 end points, there are benefits to using Sinatra, if the whole controller is short, running it in one file is good.

2. Consulting blogs and commentary you find online, identify 3 similarities between Rails and Sinatra.
- both web frameworks that can make lightweight web apps (Sinatra is simpler and lighter)
- both construct web apps with minimal code

3. Consulting blogs and commentary you find online, identify 3 things that distinguish Rails, advantages.
-Rails does things in the background automatically for your app.
-Larger scale applications with many users and 15-20 end-points and login authentication needed
-MVC based framework, coupled with a DB (Rails assumes you are using a DB, whereas Sinatra doesn't make that assumption)
-some boilerplate code setup

4. In your Rails project, what does the `routes.rb` file inside of the `/config` directory do? What does this correlate to in our Sinatra app? the controller file

5. We teach Sinatra by adding some structures that Sinatra doesn’t need, but help you make the transition between Sinatra and Rails. What does a stripped down implementation of Sinatra look like, and what are the pieces we’ve added for educational purposes? We didn't need the MVC structure with Sinatra, it could have been run all in one file, but it sets us up well to transition to Rails understanding the CRUD and MVC model taking place in the background.
