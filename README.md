Knetik Engineer Recruitment Test
==================================

Thank you for taking the time to do our technical test. It consists of two parts:

* [A coding test](#coding-test)
* [A few technical questions](#technical-questions)

Create a github repository with the following contents.

1. a single markdown file with the answers to the technical questions
2. one folder containing the technical test

## Coding Test

Knetik has a public API available at [https://recruitment-test-api.devsandbox.knetikcloud.com/devices](https://recruitment-test-api.devsandbox.knetikcloud.com/devices) that you can use to get device information, including device details.

As an example, [https://recruitment-test-api.devsandbox.knetikcloud.com/devices?filter=location:12](https://recruitment-test-api.devsandbox.knetikcloud.com/devices?filter=location:12) returns a list of devices with the location name 12, including some basic device information.

Docs for the api are located here: [https://recruitment-test-api.devsandbox.knetikcloud.com/swagger-ui/](https://recruitment-test-api.devsandbox.knetikcloud.com/swagger-ui/)

The task is to create an application that displays the following minimal information about each device.

- Connection Status
- Location Name
- Updated At

### Platform Choice

You can create the application as either a command line application or web application.  
Using Node or the Front End Javascript Framework of your choice.

Think about the type of work you would like to do at Knetik and **choose an appropriate application type**.

### Task requirements

Feel free to spend as much or as little time on the exercise as you like as long as the following requirements have been met.  

- Please complete the user story below.
- Your code should compile and run in one step.
- Feel free to use whatever frameworks / libraries / packages you like.
- Please avoid including artifacts from your local build (such as packages) in your github repo.

### User Story

As a **user running the application**  
I can **view a list of devices and filter by location, parent_location, and
connected**  
So that **I know which devices are currently online**

As a **user running the application**  
I can **render a detail view of the device listing all its properties and a section of related devices by location**  
So that **I can gain context on a devices location**

#### Bonus points

Render **Connection Status** and **Signal Strength** in a unique and attention grabbing
manner.

#### Acceptance criteria

- For the filtered device property, results are returned
- The Connection Status, Location Name and Updated Date of the device are displayed

# Technical questions

Please answer the following questions in a markdown file called `Answers to technical questions.md`.

1. How long did you spend on the coding test? What would you add to your solution if you had more time? If you didn't spend much time on the coding test then use this as an opportunity to explain what you would add.
2. What was the most useful feature that was added to the latest version of your chosen language? Please include a snippet of code that shows how you've used it.
3. How would you track down a performance issue in production? Have you ever had to do this?
4. How would you improve the Knetik APIs that you just used?
5. Please describe yourself using JSON.

#### Thanks for your time, we look forward to hearing from you!
- The [Knetik Tech team](http://github.com/knetikmedia)
