Hello! Thanks for taking a look at my responses.
Ben Karl
benkarl@me.com
719-660-0519

####Level 1:

*Bonus question! - The Agent is a server that is sent information from your machine or applications and delivers them (via the API) to Datadog so that they can be analyzed and presented back to you in our account dashboard.

#####Here are the steps I took for both Level 1 challenges:

1. $ gem install dogapi
2. From within a Ruby REPL (I use [pry](https://github.com/pry/pry))...
3. > require 'dogapi'
4. > dog = Dogapi::Client.new(my_api_key)
5. > dog.emit_event(Dogapi::Event.new("Ben Karl submitting my first event as part of the support engineer code challenge"))
  * Success! "id" => 2391716254316003247
6. > dog.emit_event(Dogapi::Event.new("@benkarl@me.com take a look see and check if this event shows up in your inbox"))
  * Success again! "id" => 2391733691530939853 (Sending emails from the event message is really cool!)

####Level 2:

1. Below is a screenshot of a graph I made tracking pageviews of a small Sinatra-based application running on localhost. The barely-visible purple line shows pageviews per second, while the blue line is tracking the system activity of my machine.

![alt text](https://p.datadoghq.com/snapshot/view/dd-snapshots-prod/org_12616/2014-07-31/a3cbc9e615b84dea5acb3171c0b4d6e4231459c7.png "Average Page Views per Second")

