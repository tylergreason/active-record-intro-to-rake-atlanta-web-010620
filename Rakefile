desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end


namespace :greeting do 
  desc 'Puts hello to the terminal' 
  task :hello do 
    puts "hello from Rake!" 
  end 

  desc 'Puts hola to the terminal' 
  task :hola do 
    puts "hola de Rake!" 
  end 
end 

desc 'does console stuff'
task :console do 

end 

task :environment do 
  require_relative './config/environment.rb'
end 

namespace :db do 
  task :migrate => :environment do 
    # require_relative './config/environment.rb'
    Student.create_table
  end 

  task :seed do
    require_relative "lib/student.rb"
 
Student.create(name: "Melissa", grade: "10th")
Student.create(name: "April", grade: "10th")
Student.create(name: "Luke", grade: "9th")
Student.create(name: "Devon", grade: "11th")
Student.create(name: "Sarah", grade: "10th")
  end 
end 