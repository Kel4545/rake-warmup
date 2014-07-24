desc "Print a nice greeting"
task :greet do
  puts "Hello there"
end

desc "Describes the time"
task :time do
  puts Time.now
end


desc "Asks for a users name"
task :print do
  puts "WHat's your name?"
  name = $stdin.gets.chomp
  puts "Hi #{name}!"
end


desc "Prints out your favorite food"
task :print_favorite_food do
  puts "Your favorite food is #{ENV['FAVORITE_SONG']}"
end


namespace :morning do
  task :wake_up do
    puts "No"
  end

  task :get_dressed => :wake_up do
    puts "so sleepy"
  end

  task :eat_breakfast do
    puts "Delicious"
  end

  task :ready_for_class => [:wake_up, :eat_breakfast] do
    puts "Nooooo"
  end
end


namespace :db do
  task :migrate do
    puts "migrate"
  end

  task :rollback do
    puts "migrate"
  end

task :default => "db:migrate"
end