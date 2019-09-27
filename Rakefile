namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end
  
    desc 'outputs hola to the terminal'
    task :hola do
      puts "hola de Rake!"
    end
  end

  desc 'console'
    task :console do
      Pry.start
    end
  desc 'environment'
    task :environment do
      require_relative './config/environment'
    end

    namespace :db do
      desc 'migrate'
        task :migrate => :environment do
        end
  
        desc 'seed'
        task :seed do
          require_relative './db/seeds.rb'
        end
      end