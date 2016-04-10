**Ruby-CommandLine-Reminder**
============================

Did You ever wonder as a geek you wold like to reminded about something through Terminal ?

**Setup**

*Ruby-CommandLine-Reminder uses Ruby 2.1.1 to 2.1.4*

* 1.Installing ruby on mac(http://code.tutsplus.com/tutorials/how-to-install-ruby-on-a-mac--net-21664)
* 2.rvm install 2.1.4
* 3.rvm use 2.1.4
```sh
 4.$gem install bundle
```
* 5.checkout the project 
```sh
$git clone git@github.com:Jai-ACrazyLearner/Ruby-CommandLine-Reminder.git
```
on project directory do 
```sh
$bundle install
```
On project directory do **$ rake -T**

it should list all the services that can be avaliable through the app

**Listing the commands**
============================
jaiprakashs-MacBook-Pro:BtTerminalApp jaiprakashgogineni$ rake -T 

```
rake timerApp:Introduction     # Introductions
rake timerApp:conclusion       # conclusion
rake timerApp:oneTimeTimer     # TimeForSingleTime
rake timerApp:paragraphOne     # para 1
rake timerApp:paragraphTwo     # para 2
rake timerApp:passageThree     # reading_passage_two
rake timerApp:passageTwo       # reading_passage_two
rake timerApp:readingTask      # reading_task_one
rake timerApp:recheck          # recheck
rake timerApp:remind_me        # remind me something {usage ==> hour=0 min=5 msg=I got to go to interview}
rake timerApp:writingReminder  # IELTS WRITING task REMINDER    
```
**Example**
============================

```sh
rake timerApp:remind_me
```
* Above task will ask you what you would like to be reminded as shown, This is effectively STDIN
```sh
what you would like me to remind you ?
```
* You may answer like this 
* remind me i have meeting in 5 min
```sh
In how many hours you would lke to reminded ?
```
* 0
```sh
In how many minutes you would lke to reminded ?
```
* 5
```sh
0-Hour:4-min:57-seconds
```
