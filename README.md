# Black Tie Attire Website

---

### Contents:

 - [Description](#description)
 - [UX](#ux)
 - [Features](#features)
 - [Technologies Used](#technologies-used)
 - [Testing](#testing)
 - [Deployment](#deployment)
 - [Credits](#credits)
---

## Description

This is a website designed to advice veiwers on how to dress appropriately for a black tie dress code. It shows all the different pieces that should be worn and informs them of the way to wear each item and which are the correct ones to be worn, it also informs them about the history of black tie and how it came to be.

This idea was due to my part time job as a sales representetive at a hackett store where many customers who came to buy suits for black tie dress code had no idea about the kind of things which they needed for this dress code so I thought an informative webpage on the do's and don'ts for this would be useful to them.
---

## UX

---

My goal in the design was to make it very traditional and antique but with a minimalistic approach as I didn't want too much clutter. Hence a grey/white/cream theme was used to create the antique feel as it is trying to represent a classic topic.
User stories:
 - I am martial arts studennt who can no longer practiice martial arts in a slub and am looking to keep up my hobby during lockdown and wish to view different price plans available for online sessions.
 - I am martial arts studennt who can no longer practiice martial arts in a slub and am looking to keep up my hobby during lockdown and wish to subscribe to a advanced level course which provide online sessions to help me keep practice for my grading.
 - I am a parent who wishes to find a way to help my child keep occupied during lockdown and wish to browse for sporting activities which the child can do from home with prospects to continue the training in a studio in person when lockdown finishes.
 - I am a parent who wishes to find a way to help my child keep occupied during lockdown who wants to sign my child up for a begginers course in martial but wish to cancel the subscription when lockdown is over as he will not have as much free time.
 - I am someone not looking to subscribe to online sessions for martial arts but am looking to find a dojo near me to join when lockdown is over.
 - I am the owner of the site and wish to view the mailing list for subscriptions.

---

## Features

### Existing Features

 - A list of subscription plans with prices and descriptions are available for users to look at to compare with other subscription plans.
 - The ability to subscribe and be added to the mailing list of the club for weekly sessions.
 - There is a admin login and registration function using django superuser.
 - Django superuser can have access to view all of the purchases made on the website to view the mailing list and which subscription each person has purchased.
 - Users have the ability to sign up to the website and purchase a subscription plan.
 - Subscribers have the ability to change or cancel their subscription plans. 

### Feaatures left to impend

 - Free trial videos could be added to the website so that people get a chance to see the kind of sessions they will recieve from their subscriptions, this was not added as access to any existing videos was not available.
 - Friendlier ux for purchases, the default stripe payment url is used in this website, a unique one could be created and implemented.
 - Access to the email provided in the link was not available so confirmation emails are sent from a fictional address.
 - Better quality photos would help keep the styling cleaner.
 - UPDATE - On the night before submission was due my computer crashed before I had a chance to commit the changes from the subscription method and payment form, the stripe usage is there but not functional with the submit button in checkout.html form, due to lack of time to go over again I have been unable to fix it as I had tried many different methods and couldn't put together the method which had worked fro me.
---

## Technologies Used

 - HTML
 - CSS
 - Bootstrap (4.2.1)
 - Features
 - This site uses the scrollSpy feature in Bootstrap. 
---

## Testing

Browser compatability: - Go to the "Membership Plans" page.
              - Select a subscription plan.
              - Click subscribe.
              - Try to submit the empty form and verify that an error message about the required fields appears.
              - Try to submit the form with an invalid billing address and verify that a relevant error message appears.
              - Try to submit the form with an invalid card number and verify that a relevant error message appears.
              - Try to submit the form with all inputs valid  using test card 4242 4242 4242 42424 24/24 424 and verify that a success message appears.

Cancel Subscription: - Go to profile page of user
             - Clcik cancel subscription.
             - Go to superuser.
             - Check that the subscription is canceled from the test user.

Register User: - Add register to navbar.
     - Go to sign up under account icon.
     - Try to submit the form with empty fields and verify that a relevant error message appears.
     - Try to submit the form with an invalid password and verify that a relevant error message appears.
     - Type valid username and password.
     - Click 'Add user' - If success you would be taken to the index.html page and session=user would be in session, if not various errors could happen.
     - To fix any errors check run.py and links in the register form from register.html and try again.

Login User: - Add login to navbar.
     - Go to login under account icon.
     - Try to submit the form with empty fields and verify that a relevant error message appears.
     - Try to submit the form with an invalid password or username and verify that a relevant error message appears.
     - Type username and password created from sign up form.
     - Click 'Login' - If success you would be taken to the index.html page and session=user would be in session, if not various errors could happen.
     - To fix any errors check run.py and links in the register form from register.html and try again.

## Deployment

This site is hosted using GitHub pages, deployed directly from the master branch. The live site updates automatically each time there is a new push to the repository. You can git clone the code to run it locally on your machine.


There is no differences between the deployed version and deployment version.

---

## Credits

### content:
 - The contents are about black tie and were written off my own knowledge from previous work in a menswear store, but https://en.wikipedia.org/wiki/Black_tie was used to help me explain the history aspect.

### media:
 - Most of the photos were taken from https://www.hackett.com/gb/home with 1 photo from https://www.prada.com/gb/en/men/shoes/lace-ups.html, this is because I was unable to find suitable photos elsewhere on open source websites and so have credited these website in the footer.

### Acknowledgements:
 - I used W3schools and the boostrap website to help with dividing my colums properly and making the cards in the accesories section.