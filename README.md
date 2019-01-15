# Wolt Coding Task 2019 - *"Pickup times"*

This coding task is meant for those aspiring engineers who are applying
for Wolt's Engineering Internships in 2019. Optionally you can send us a
link to your Github profile (containing existing projects) or any
example of your code in any format of your preference, and skip this
exercise altogether. Find the details to apply
[here](https://hire.lever.co/jobs/internal/527274e5-f0ab-4ed7-842b-5c61cb137529),
deadline to apply is 17.2.2019.

---

Our courier partners are one of the main pillars of successful Wolt
operations in 38 cities covering 14 countries (and growing fast!).
Courier partners use Wolt's own mobile application that feeds them new
tasks, allows reserving shifts, shows earnings and keeps everyone
informed about the status of the city. The mobile app communicates with
the backend where we have a pile of Scala, C++ and Python code
constantly optimizing best delivery scenarios so that the operation will
run smoothly and efficiently.

Wolt's delivery task is split into two parts: *pickup* and *dropoff*. A
*pickup* task means driving to a restaurant, collecting the prepared
food, putting it to a heat bag and then continuing with the next thing.
A *dropoff* task covers the rest of the delivery - taking the food to a
customer with a smile.

In this coding exercise we are going to focus on pickup tasks. When a
customer buys food through Wolt, the first thing that will be done is to
calculate a pickup time. A pickup time indicates how many minutes it
will take for our courier partner to arrive to that specific restaurant.
There are many factors to take into consideration:

-   How many courier partners are available in the city
-   How busy are courier partners
-   How are courier partners located in relation to the restaurant

Obviously the busier the city is, the higher the pickup time. Very
central areas of a town might be faster to reach, but they also often
contain the most popular restaurants (biggest rush). On the other hand
restaurants on outer areas of the town might have less orders, but they
will require more travel time.

Your task is to help one of our courier operation managers to analyze
pickup times. The courier operation manager has sent you a following
message:

>I would like understand what is the **median pickup time** for each
>restaurant between certain hours (e.g. 15-16). The data set of
>pickup times has been collected from Helsinki between 7.1. -
>13.1.2019.
>
>- [locations.csv](http://summer2019.wolt.com/Helsinki/locations.csv)
>- [pickup_times.csv](http://summer2019.wolt.com/Helsinki/pickup_times.csv)
>
>The first file contains all pickup locations (restaurants) in Helsinki 
>and the second one all pickup times from that week.
>
>I would like to have either an command line application **or** some
>kind of graphical user interface. Whichever you want to create. I need to be 
>able to select the day and start / end hours when
>using the program.
>
>The command line program could work something like this:
>
`$ median_times Helsinki 07-01-19 19-20 mediantimes.csv`
>This command would calculate medians of pickup times for all locations
(in Helsinki) between 19-20 on Monday 7.1 and store times to a CSV
file (example below).
>
```
location_id,median_pickup_time
1,21
2,15
3,6
etc.
```
>
>If you rather build a graphical user interface instead of the command
line application, then here is my idea about that one.

![UI example](http://summer2019.wolt.com/helsinkimap.png "Pickup times UI example")

## Practical things

-   You can use **any programming language and 3rd party libraries you
    want**. However, we will really appreciate if you can write your
    solution with either Python, JavaScript or Scala (languages mostly
    used by Wolt).
    
-   When you are ready, leave us an application
    [here](https://hire.lever.co/jobs/internal/527274e5-f0ab-4ed7-842b-5c61cb137529)
    accompanied by your solution (stored in a GitHub repository or if
    in other format, send your code to laura\@wolt.com)
    
-   You need to build either an command line application or a graphical
    user interface (no need to do both). Examples above are just that,
    examples. Feel free to do a better design on how the input can be
    given to the program.
    
-   The courier operation manager is only interested about median times
    between certain hours (without minutes). So there is no need to
    handle exact timestamps in this first MVP.

## Consider also following

-   We need to be able to test your program. So please provide good
    instructions how to get everything running smoothly.
    
-   Everyone at Wolt loves clean code :)

-   The courier operations manager probably wants to use your program
    also with other cities, so it might be a good idea to make the
    location of the data configurable.

If you have any questions about the task, don't hesitate to contact our
Product Recruitment Manager at <laura@wolt.com>

## One final disclaimer

The data in this task **is not real** - coordinates do not point to real
restaurants and pickup times have been fabricated. If you want to see
how our system performs in real-life, impress us with your solution and
come work with us!

### Happy coding!
