# stupid-simple-api
A stupidly simple API. Just serving simple JSON files.

# Why?
I did this to see for myself if it was possible.

I also learned why we don't do it this way but use a server instead.

## So why shouldn't we do it this way, when it is so easy and simple?
Well, for practice purposes or for quickly serving up some dummy data that ultimately needs to be replaced before production anyway, it is perfectly fine to do it this way.

But, imagine, for example, we have data for thousands of restaurants, and each restaurant has loads of data:
- info about the restaurant
- info about employees
- menu(s), with detailed info about each meal
- location
- whatever

We are dealing with hundreds of thousands of lines of data here.

Say we need to fetch data for one restaurant to get info about their location?
To get that info we would need to fetch ALL data for ALL restaurants, and then filter the data to get the info we need!

Say the size of the data is 1MB but data for the location of that one restaurant is only 1KB, that is a lot of unnecessary data we are sending across the internet.

To get around that we need a server that can filter the data before we send it!

So to say it very basically; we don't do this for performance reasons.

Thank you for reading this :-)
