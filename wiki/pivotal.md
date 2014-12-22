## pivotal

### pivotal - github integration

You can integrate Github with Pivotal. When somebody commits some changes connected to this ticket, a comment will be added to this ticket. In this way you know who, how and when is/was working on a ticket.

You need to be the repo admin on Github and you need the Pivotal project owner's token.

Here is the link how to make the integration: http://www.pivotaltracker.com/community/tracker-blog/github-service-hook-for-pivotal-tracker

### dev's work flow - pivo_flow gem

The commits always have a message. To make the integration know which commit is connected to which ticket you need to include the ticket number in the commit message, like: `registration added [#123456]`. But it's boring to add the number each time you commit your changes, so the `pivo_flow` gem will help you.

Link: https://github.com/lubieniebieski/pivo_flow

To install and cofigure just read the readme and follow the instructions. You can find your token on Pivotal -> click on your user name -> Profile -> the token is on the bottom.

In everyday dev's life:

1. `pf start <ticket number`
2. you make commits without remembering the ticket's number
3. when you want to work on another ticket: `pf start <another number>`

