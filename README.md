>**Note**: Please **fork** the current Udacity repository so that you will have a **remote** repository in **your** Github account. Clone the remote repository to your local machine. Later, as a part of the project "Post your Work on Github", you will push your proposed changes to the remote repository in your Github account.
# Project Title

## Motivate BikeShare System Data

The project uses data provided by [Motivate](https://www.motivateco.com/). 

### Date created

Date: Tuesday September 28, 2021

### Description

 This project uses data from a bike share system provider for many major cities in the United States, to uncover bike share usage patterns. The project computes the system usage between three large cities: Chicago, New York City, and Washington, DC.This project computes data from Chicago, New York City, and Washington provide descriptive statistics on the following information:

* Popular times of travel (i.e., occurs most often in the start time)
  * most common month
  * most common day of week
  * most common hour of day

* Popular stations and trip
  * most common start station
  * most common end station
  * most common trip from start to end (i.e., most frequent combination of start station and end station)

* Trip duration
  * total travel time
  * average travel time

* User info
  * counts of each user type
  * counts of each gender (only available for NYC and Chicago)
  * earliest, most recent, most common year of birth (only available for NYC and Chicago)

### Files used

This following files have not being included into the repository because of their size but they are available upon request. To get the solutions to all descriptive statistics the following dataset from the cities were used: 

* chicago.csv
* new_york_city.csv
* washington.csv

### The main Function

 `` def main():
    while True:
        city, month, day = get_filters()
        df = load_data(city, month, day)

        time_stats(df)
        station_stats(df)
        trip_duration_stats(df)
        user_stats(df)

        restart = input('\nWould you like to restart? Enter yes or no.\n')
        if restart.lower() != 'yes':
            break


if __name__ == "__main__":
    main() ``

 
### Credits

This project was inspired by repository from the [Udacity](https://github.com/udacity/course-collaboration-travel-plans) course. 

I would also like to give credit to the [Github documentation](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#paragraphs) on how to properly format the README.md file. 