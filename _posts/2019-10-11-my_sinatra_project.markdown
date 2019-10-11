---
layout: post
title:      "My Sinatra Project."
date:       2019-10-11 17:35:21 +0000
permalink:  my_sinatra_project
---

My sinatra app lets users record rock climbing routes / boulder problems they have discovered (or bolted in terms of sport climbing) which are added to a public list of community recorded climbs.

I want this blog to less technical and more about my thoughts and what I learned  from this project in terms of having a clear idea about what my program is going to be about before I start and trying to break down the week into individual days of work to smooth out the peak of potential stress... and how all of the above failed but made my experience so much better. 

If you're reading this heading into your own project week looking for tips or inspiration I'm going to start off saying to take the first day or two of your week to do some hardcore revision. Honestly it's impossible to put a price having a serious refresh before building something from the ground up I'd recommend the three big video reviews leading up to the project in the curriculum which are the Forms, Authentication, and Pirates lab video reviews. 
Re-watching these really put me in a comfortable state of mind when having to run through my MVC patterns and I even played them as background sound while doing my work so Avi's voice so cheerfully narrate my descent into madness "This is really fun, I'm having a great time". 

So our research days are over and it's time to start building and after day one I was feeling pretty confident. I had build out the the app structure starting with `config.ru`  follow up with `environment.rb` inside a `config` folder, the `Gemfile` (containing `sinatra`, `rake`, `shotgun`, `tux`, `activerecord` etc), the `Rakefile`where we later mount our `controllers` and finally linking everything together with `require` and `require_relative`.

After running `bundle install` I setup my tables through `rake` and `activerecord` followed by their `models` the corresponding `controllers` plus our `ApplicationController` and the first set `views` so I could start testing my code. This is the pattern we live by for the duration of this process working through the **MVC** flow ticking off **C**reate **R**ead **U**pdate **D**estroy until the `spec.md` is satisfied, many hours and six mugs of coffee later(I have a 500ml mug which I highly recommend) we are setup going into day two with only **U**pdate and **D**estroy left to implement. 

Alright day two is here and we've only a bit of functionality left before my program is done(or so I thought). I haven't gone into extreme detail of the process because I did want this to be less technical but atleast outlining how we got to this stage feels necessary, during out setup on day one we created the `UserController` which houses all of our user functionality and this is where I made a fatal mistake, I had forgotten to create a `session` to `user:id` link so even though I had all of the `user:id` verification required for the project it was all broken and I had no idea why. 

Now this is where I had my breakthrough and I feel like other people who are in the first month or two of these courses where self doubt in our ability to learn and program are very potent. 
I came to the realization that even though I had been stuck for hours I had been totally focussed for hours. 

Frustrated beyond belief yes but bored? Not even for a second. 

I finally understood the mentality of "When a program breaks it's a good thing because it's the first step in making it work." and how frustration turns into excitment so quickly are you weed out each little error until everything just works. 
I never thought I'd be so happy to see **sinatra doesn't know this ditty** because now it means "Everything works up until this route so stub out this method and we go from there." while before it meant "I messed up somewhere, I don't understand, I'm such an idiot.".

It's knowing that for each moment of doubt when you hit a wall there is an equally powerful moment of celebration when you discover the solution. 

Two days, eleven mugs of coffee, and one epiphany later and you've got a program.





