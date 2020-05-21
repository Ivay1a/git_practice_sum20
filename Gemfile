# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem 'colorize'

require 'colorize'def puts_git(cmd)
  puts `git #{cmd} -h`
  menu
enddef menu
  puts 'Main Menu'.colorize(:cyan)
  puts '1: Enter git command'.colorize(:cyan)
  puts '2: Exit'.colorize(:red)
  choice = gets.to_i
  case choice
  when 1
    puts 'Enter git command'
    puts_git(gets.strip)
    menu
  when 2
    exit
  else
    puts 'Invalid choice'
    menu
  end
endmenu
