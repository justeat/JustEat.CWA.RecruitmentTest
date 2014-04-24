Consumer Web Applications Recruitment Test
===========================================

Thank you for taking the time to do our technical test. It consists of two parts:

* Coding test
* A few questions

# Coding Test

JUST EAT has a public API available at http://api-interview.just-eat.com/ that you can use to get restaurant information, including which restaurants deliver to what areas.

As an example, http://api-interview.just-eat.com/restaurants?q=se19 returns a list of restaurants that deliver to an outcode, including some basic restaurant information (for outcode = se19).

The API requires you specify a set of valid request headers before it'll respond.

		Accept-Tenant: uk
		Accept-Language: en-GB
		Accept-Charset: utf-8
		Authorization: Basic VGVjaFRlc3RBUEk6dXNlcjI=
		Host: api-interview.just-eat.com

##Coding Test 1

The task is to create a ASP.NET MVC Web application using C# which consumes our public API. 

This application should:

1. allow users to search for a postcode manually
2. search results should display the following for each restaurant that delivers to that postcode
	* Name
	* Average rating
	* Restaurant logo
	* Cuisine Types
3. allow users to sort results by Name or Average rating (Client Side)

### Task requirements

- All requirements to be completed with an appropriate level of testing.
- Feel free to use whatever javascript, testing, mocking/stubbing frameworks you prefer, along with any other packages.
- Your code should be of production quality.
- Please include a readme file on how to get your application up and running
 
##Coding Test 2

Write a function that will pass the following Jasmine test for a basket total calculator (please feel free to extend the test criteria to ensure it is fit for purpose).

		describe("basket total calculator", function () {
			var basketCalc = new BasketCalculator();
			it("Can add items to the basket total", function () {
				expect(basketCalc.add(2.3)).toEqual(2.3);
				expect(basketCalc.add(1.3)).toEqual(3.6);
				expect(basketCalc.add(5)).toEqual(8.6);
			});
			it("Can remove items from the basket total", function () {
				expect(basketCalc.remove(2)).toEqual(6.6);
				expect(basketCalc.remove(2.6)).toEqual(4);
			});
		});


# Questions

* Did you have time to complete the coding test? What would you add to your solution if you had more time?
* What's your favourite programming language? Why?
* How would you track down a performance bottleneck in a .NET application? Have you ever had to do this?
* List a few of your prefered Javascript frameworks (also let us know in which situations you would choose to use/not use them)
* Please describe yourself using either XML or JSON.


In order to avoid bounced emails we would like you to submit your results by uploading the relevant zip file to a shared Google Drive folder. Please send an email to tech.recruitment@just-eat.com with your **valid Google email address** so we can give you the correct upload permissions.

Thanks for your time, we look forward to hearing from you!

