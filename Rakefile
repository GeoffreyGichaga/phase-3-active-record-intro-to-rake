namespace :greeting do 
  desc 'outputs hello greeting on the terminal'
  task :hello do 
    puts 'hello from Rake!'
  end 

  desc 'outputs hola greeting on the terminal'
  task :hola do 
    puts 'hola de Rake!'
  end 

end











namespace :db do 

desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  desc 'accessing the configuration file'
  task :environment do 
    require_relative './config/environment'
  end

  desc 'seed the database with some dummy data'
  task seed: :environment do 
    require_relative './db/seeds'
  end 

  
end 

desc 'drop into the pry console'
  task console: :environment do 
    pry.start 
  end 
 
