# Coding Assessment Questions

**1: Q. How long did you spend on the coding assessment? What would you add to your solution if you had more time? If you didn't spend much time on the coding test then use this as an opportunity to explain what you would add.**
        **A.** I'm not quite sure, I was really timing myself and I was doing a lot of other things at the same time. I had a lot of interruptions while working on it. I spent maybe a couple hours total on it.  If I had more time, there are ton of things than can be done to this. Error checking, what if I don't get a response from the API? Caching results so I don't have to hit the API when paging back and forth, so when loading devices from a single location if I've done so before. A programmer could spend days tweaking something like this.
   
<b>2: Q. What was the most useful feature that was added in the latest version of your chosen language? Please include a snippet of code that shows how you've used it. </b>
   **A.** In ES6 they introduced `isInteger()` and `isNaN()` and `isSafeInteger()` functions. I didn't use them in the page I wrote, as I didn't spend the time to do any error checking in the javascript. 
		If I had spent time for error checking, instead of just doing (inside the paging functions)  `var current_page = parseInt(pagenumber.innerHTML);` I would have done 
		`(if (isSafeInteger(pagenumber.innerHTML) { /* do the paging thing */ } else { /* handle bad data */ } `

<b>3: Q. How would you track down a performance issue in production? Have you ever had to do this? </b>
   **A.** The best way to track down a performance issue in producttion, is to first actually use the application in question. Then you need to mirror the problem in the development environment. From there you would need to 
		test various parts of code with usually larger data sets to see which pieces of code are the most sluggish. If none are them specifically slow, maybe there is an integration issue that has a cumulative effect on 
		performance. With web development the problem could be a bandwidth issue for the client or something with the client's machine. Then you need to think about how to solve that. In my experience, there is usually an
		ineffienct loop somewhere, or a SQL query is slow due to many tables scans becuase of unneccesary DISTINCTS or SELECT (*) commands. I had an application have terrible performance because every click needed to make a round
		trip to the server and the client's bandwith was just awful, so even checking a radio button would take like three seconds or so to reload the page. Once I became in charge of the application, one of the things I made sure
		to do was start including javascript into the web application and rewrite some of the back-end code so it was indifferent to specific elements showing or being hidden on the page, and to return a minimum about of data as possible
		for the web application to function.
	
<b>4: Q. How would you improve the Knetik APIs that you just used?</b>
   A. Returning the page number would be useful with the way it currently works. I don't think you need the filter command, as using location=10 should automatically filter for those locations.
   
<b>5: Q. Plese Describe Yourself Using JSON <br>
	A. `{ "FirstName": "Charlie", "Lastname": "Johnson", "Occupation": "Senior Software Developer", "Hobbies" : [ "Board Games", "Reading" ], "Pets" : [ {"Name" : "Ace", "PetType" : "Dog" }, {"Name" : "Riku", "PetType" : "Dog" }, {"Name": "Dexter", "PetType" : Dog" } ] }`
	
