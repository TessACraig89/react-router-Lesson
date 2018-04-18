
<!--
Creator: <Name>
Market: SF
-->

![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png)

# React Router

### Why is this important?
<!-- framing the "why" in big-picture/real world examples -->
*This workshop is important because:*

React is a framework for building single page apps (SPAs). In order to prevent the browswer from reloading the page to display new views, we need to give the browser an alternate system. React router is the system that specifies which components should display at each URL.

### What are the objectives?
<!-- specific/measurable goal for students to achieve -->
*After this workshop, developers will be able to:*

- Distinguish between a standard web page and a single page app (SPA)
- Illustrate the difference between server side routing and client side routing
- Write the basic syntax of the Route component to associate a URL and a component.


## Review
What different types of server requests are required to actually display a website? How many?

## What is React Router?

It's a package that allows us to change the URL, making it _look like_ the user is visiting different pages, when they are _actually_ still on the same page. This is a common pattern in Single-Page Applications ( **SPA** s).

## So what does it do?

It takes care of two tasks that are traditionally accomplished by going to different pages.

1. It keeps track of what is supposed to happen, and which components should be rendered, when you visit specific URLs.
2. It updates the browser's history with those URLs.

The second piece happens automatically; the first part is what you have to set up. Setting up routes for the React router is very similar to setting up routes in Express. You define the same basic things: the path, and what should happen when that path is visited. The only difference is that it will do the routing _on the client_, without actually hitting your server.

## How does it look?

We'll break it down step by step in the lab, but here's a quick code example of two routes from this afternoon's lab: 

```html
<Route exact path='/' component={ Home }/>
<Route path='/todos' component={ TodosContainer }/>
```
