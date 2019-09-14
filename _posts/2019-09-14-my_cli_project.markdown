---
layout: post
title:      "My CLI project "
date:       2019-09-14 12:26:35 +0000
permalink:  my_cli_project
---



My first experience with project week really gave me the full spectrum of emotions ultimately governed by coding, 
the lowest lows and the highest highs all brought you by symbols and characters sat infront of you in your environment.

I have two  major hobbies in my life one being rock climbing and the other being starcraft so it was only natural to build the program around one of the two. 

In the end I went with starcraft specifically a simple program that can tell me the upcoming tournaments in the professional starcraft 2 circuit and set about creating the gem, luckily a lot of this process is taken care by using **bundle gem "gem name"** followed by running the through our **git** commands setting up the repository and linking everything together to save our work from untimely crashes(remember kids *commit early and often*).

With the data structure setup it was time to start creating the program, after watching all of the relevant walkthroughs and live lectures the most straight forward way for the gem to complete it's task is to split it into two parts, the **interface** where the user can access the date and the **scraper** which is collects the data from our chosen website.

With that in mind if I have data that has been scraped but no way to interact with it then whats the point? Therefore the **interface** comes first.

If you are someone browsing Learn magazine in search of help with this project I'd highly recommend approaching it in this way because we can easily test our **interface** by using fake data.  

So now we create three new files.
 In `lib` we create `cli.rb` for our interface, `game.rb` to house our fake data and eventually our scraper and in `bin` pc_games which will serve as our **executable**.
 
 I settled on a pc_games naming scheme simply because it's a bit easier to with vs sc_tournaments. 
 
Taking the example from the CLI project walkthrough and repurposing the `pc_games.rb` to act as our environment using `require_relative` to link all of our files together as well adding `require` for **nokogiri , open-uri, and pry** for our scraper later on.

And finally creating and the necessary classes and relating them together with `::` e.g. `PcGames::CLI.new.call` in our `bin` file which is what invokes the our program. 

Now that the skeleton of the program is in place started on the interface by first filling the `PcGames::Game` class with a set of fake data mirroring the future real data that the interface would call upon.
Now in the `PcGames::CLI` class I created a start up method with the programs initial prompts then the program's reactions based on the user's input and finally a simple method for when the user enters an unrecognized input or wants to exit the program.
Now with the interface done we replace our fake data in the `PcGames::Game`with real data from our website by creating scraping methods using **nokogiri** which push their collected data into an array which the interface can call upon.


Ultimately this first project was a real wake up call in terms of how much more planning and focus that needs to go into something like this and the real champions of this project being the lessons leading up to it in the curriculum because even if you go in feeling like you have nothing to go on if you relfect on those previous lessons they can push forward and to the finish. 







 
 
 

