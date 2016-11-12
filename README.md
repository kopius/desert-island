# Desert Island

In today's world of unlimited data plans, gigs upon gigs of storage space, and social media feeds that push new photos off the page faster than you can upload them, we wondered...

...what if an online photo album only let you upload five images?

Not because of storage limits, or arbitrary usage fees, but simply as an exercise in self-definition and discipline. How would you sum yourself up in five pictures?

The idea for our app rose up out of this question. If you were stranded on a desert island with nothing but your wits and a 4G smartphone, what five image files would you want to have stored in the cloud? If these photos were the only way you could communicate with your fellow castaways on distant shores, what would you want them to see?

Introducing...**Desert Island.**

## Screenshots

Coming soon!

## Technology

The Desert Island client is a single-page web app written in HTML5/CSS3/JavaScript. Server calls are handled with jQuery/AJAX. Styling is done with a combination of Sass and Bootstrap. Dynamic rendering of content is done via Handlebars templates.

The back end ([repository here](https://github.com/kopius/desert-island-api)) is a Node/Express API that stores user info and file metadata with MongoDB via Mongoose middleware and mLab. Photos are uploaded to an Amazon Web Services S3 file bucket using the aws-sdk Node module.

All dependencies are managed with NPM.

## Development

Desert Island was originally developed by myself and three others as a group project at General Assembly. We began with a simple goal: to build and deploy a full-stack web app that allows users to upload, manage, and share files. Before writing any code, we expanded that goal into a shared vision of restricting users to photos only, and a maximum of five uploads. The 'Desert Island' concept emerged from this early planning stage.

Team members worked together on both the client and API using a centralized Git workflow. Each developer was assigned specific roles in order to streamline development, but everyone contributed code to both the front and back end. The two halves of the app were built in tandem, with the team working in pairs at a single table to facilitate communication. This allowed us to build the app's core functionality very quickly. It also meant we could bring our combined powers to bear on any bugs or issues that arose.

We tackled the solo-user stories first, making sure a user could upload and manage photos before moving on to the sharing feature. Once we had working templates for displaying a user's 'island', it was relatively easy to add a 'read-only' template and a sidebar for browsing other users' islands.

#### Development Materials

These materials offer further insight into the development process for Desert Island:

[User Stories](docs/stories.md) | [Wireframes](docs/wireframes)


## Next Steps

This fork of the Desert Island project will incorporate several additional features in its next release:

#### Social

Desert Island currently lets users browse other islands at random. I'd like to make this feature more focused and social by allowing users to designate each other as friends and limit the privacy of their islands to friends-only if they choose.

#### Improved UI

The user interface needs to be tightened up a bit. The next version of Desert Island will have more cohesive styling and a separate view state for single images.
