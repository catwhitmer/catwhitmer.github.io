---
layout: post
title:      "My CLI Gem Project"
date:       2020-03-08 20:11:48 +0000
permalink:  my_cli_gem_project
---


For this project we were required to scrape a website for information and insert that information into a gem using object-oriented ruby. My first idea was to find an animal rescue website to scrape because I absolutely love animals, especially dogs.  I found a really great website that really inspired me to make this project.


**Getting started**
The first step was to find a website and plan out what kind of information I wanted my gem to display. The goal was for the gem to display dogs that were available for adoption and give the user the choice on which dog they could get more information about. It was also important to include the ability for the user to exit the program and still have access to the dogs at any point. After figuring out what I wanted the gem to do, it was time to set up the gem using bundler.

**Setup**
I used bundler to set up my file structure, but there many other ways to set them up. Bundler was very easy to install and  it created all the files in a nice structured manner. 

* After you open sandbox you can create your gem using the following code:
```
bundle gem name_of_gem
```

* Then it's time to cd into your gem so that your code will be saved in it instead of the sandbox:
```
cd  name_of_gem
```

**Github**
 The next step is to connect your gem with github. Github makes it really easy to connect your gem by walking you through it step by step.

First you create a new repository by pressing the new repository button in the top right corner of your screen.
Then you add each line of code into your sandbox terminal.
```
git add .
git commit -m "first commit"
git remote add origin https://github.com/username/your_gem.git
git push -u origin master
```
Then its time to code!


**Coding**
The first thing I did is write everything out in pseudo code. In doing so, I had a sense of how everything was going to come together. Then all of the code was divided into three classes: the CLI class, the Scraper class, and the Dogs class.

* The CLI class contains all of the code that the user interacts with including a welcome and goodbye message. It also houses the final code for the scarped information.
* The Scraper class includes two methods: the scrape_dogs method scrapes the first level data of all of the dog names with their matching url. The scrape_dogs_detail method scrapes all of the dog’s detailed information including breed, age,etc. Both methods used nokogiri and open-uri to extract the information.
* The Dogs class includes the initialize method and stores all of data using the @@all class variable.

```
class DogAdoption::CLI 
  
  
  def start 
    puts "\nWelcome to Cat's Dog Adoption!".light_green.bold
    puts "\nFor a list of dogs available, type list."
    puts "To leave anytime, type exit."
    dog_menu
  end
```

**What I learned**

This project really taught me a lot. It helped me to better understand how all of the code works together.  A few things that stood out were:

* Save often
* Make sure your website is scrapable
* Binding pry is your best friend
* Take breaks




