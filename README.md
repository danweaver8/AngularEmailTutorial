# AngularEmailTutorial
This was getting familiar with more angular models, directives, factory, controllers etc. This was an email type example. Since I've done a few angular tutorials I already had node installed and was able to use npm for the dependencies.This made adding angular, jquery, angular-routing, and angular-sanitize quite easy.

It was a good walkthrough first creating what the defined angular app will be. We next added the InboxCtrl which ended up being a main controller. Next, a little test controller was added to ensure that node and angular were up and running.

Next we took the html out and added the ng-view which tells the browser that we are going to inject HTML based on the url we are visiting. This requires us to make a global app.js file which included the angular app we defined in the index.html along with the  included extensions such as route and sanitize. We defined the URL template, controller, and an alias.

We next created an inbox.html file which is what will be injected in when the user first navigates to the app. Next we created a inbox control file. Next, a inbox factory file was created. This contains the behavior for the inbox such as going to a message, loading the message, and deleting the message. This caused us to connect the factory and the controller.

In our Inbox.html we have an '''<inbox></inbox>''' which is a directive that we created next. We defined the behavior of the inbox with the control and template for the inbox template. So we now have an inbox factory, inbox directive, inbox control, and an inbox template.

The next thing I did was replicate the same functionality but for the email. This means viewing an email, replying, going back, etc. We also added the cloaking so elements such as {{title}} as invisible. Also added angular sanitize to use the ng-bind-html="email.message.content" which binds html from the json which had <p> tags.
