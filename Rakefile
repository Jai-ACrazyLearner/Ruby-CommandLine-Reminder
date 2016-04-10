require 'rubygems'
require 'thor'
require 'colorize'
require 'timers'
require 'clockwork'
require 'rake'
require 'hirb'

namespace :timerApp do
  #========================================================================================
  # Reading Task
  #========================================================================================
  #task for timer to reapeat same time again
  desc "reading_task_one".red
  task :readingTask do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say 20 minutes have been started for passage one`
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say 20 minutes have been finished for passage two, and you have 10 seconds break`
        sleep (10)
        break
      end
    end
    if startTime.min == 0
      break
    end
    sh "rake timerApp:passageTwo"
  end
#Task two
  desc "reading_passage_two".red
  task :passageTwo do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say 20 minutes have been started for passage two`
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say  20 minutes have been finished for passage two, and you have 10 seconds break`
        sleep (10)
        break
      end
    end
  end

#passage three
  desc "reading_passage_two".red
  task :passageThree do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say  20 minutes have been started for passage passageThree`
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say 20 minutes have been finished for passage passageThree, and that is your end od writing test`
        sleep (10)
        break
      end
    end
  end

#========================================================================================
# Reading Task
#========================================================================================
#Task two for single time
  desc "TimeForSingleTime".red
  task :oneTimeTimer do
    min = ''
    STDOUT.puts "how many minutes you wnated counter for ?".red
    min = STDIN.gets.chomp
    hour = ENV['hour']
    min = ENV['min']
    msg = ENV['msg']

    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        puts "Suchitra Your #{min} minute time is finished for #{msg}"
        `say "#{msg} Your selected time is finished, You should stop now what you menat to be doing"`
        `say  "Suchitra Your #{min} minute time is finished for #{msg}"`
        sleep (30)
        break
      end
    end
  end


#Remind me some thing
  desc "remind me something {usage ==> hour=0 min=5 msg=I got to go to interview}"
  task :remind_me do
    msg = ''
    STDOUT.puts "what you would like me to remind you ?".red
    msg = STDIN.gets.chomp
    hour = ''
    STDOUT.puts "In how many hours you would lke to reminded ?".green
    hour = STDIN.gets.chomp
    min = ''
    STDOUT.puts "In how many minutes you would lke to reminded ?".red
    min = STDIN.gets.chomp

    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, hour, min, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        puts "Suchitra here is the reminder and it's time to takoff for = " + "#{msg}".red
        `say reminder "#{msg} . OK now stop what you doing do what you asked for "`
        break
      end
    end
  end
#======================================================================================
#### Reading Module
#======================================================================================
#Reading Timer Planning
  desc "IELTS WRITING task REMINDER".red
  task :writingReminder do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your Five minutes planning is started`
    every_so_many_seconds(1) do
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your Five minutes planning is finished`
        break
      end
    end
    sh "rake timerApp:Introduction"
    sh "rake timerApp:paragraphOne"
    sh "rake timerApp:paragraphTwo"
    sh "rake timerApp:conclusion"
    sh "rake timerApp:recheck"
  end
# Introduction
  desc "Introductions"
  task :Introduction do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your Five minutes Introduction is started`
    every_so_many_seconds(1) do
      puts "jai"
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your Five minutes Introduction is finished`
        break
      end
    end
  end
# Para 1
  desc "para 1 "
  task :paragraphOne do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your 10 minutes Paragraph one is started`
    every_so_many_seconds(1) do
      puts "jai"
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your 10 minutes Paragraph one is finished`
        break
      end
    end
  end

# Para 2
  desc "para 2"
  task :paragraphTwo do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your 10 minutes Paragraph two is started`
    every_so_many_seconds(1) do
      puts "jai"
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your 10 minutes Paragraph two is finished`
        break
      end
    end
  end

#conclusion
  desc "conclusion"
  task :conclusion do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your 5 minutes conclusion is started`
    every_so_many_seconds(1) do
      puts "jai"
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your 5 minutes conclusion is finished`
        break
      end
    end
  end

# recheck
  desc "recheck"
  task :recheck do
    def every_so_many_seconds(seconds)
      last_tick = Time.now
      loop do
        sleep 0.1
        if Time.now - last_tick >= seconds
          last_tick += seconds
          yield
        end
      end
    end

    $counter = 1
    `say your 5 minutes recheck is started`
    every_so_many_seconds(1) do
      puts "jai"
      puts `clear`
      #YYYY-MM-DD-HH-MM-SS format
      startTime = Time.new(2016, 01, 31, 0, 1, 0)
      startTime = startTime - $counter
      puts "#{startTime.hour}-Hour" + ":#{startTime.min}".red+"-min" + ":#{startTime.sec}-seconds".red
      $counter = $counter +1
      if startTime.min == 0 && startTime.sec == 0
        `say your reading task is finished`
        break
      end
    end
  end
end


namespace :ruby_env_files do

# recheck
  desc "recheck".red
  task :recheck do
    STDIN.raise










  end
end
#### Reading Module


