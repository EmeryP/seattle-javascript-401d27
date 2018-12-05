![CF](http://i.imgur.com/7v5ASc8.png) LAB - Authentication
==========================================================

## Before you begin
* Fork [this sandbox](https://codesandbox.io/s/1rp021q45q)
* Install and start the API server (found in the class repository) for local end to end testing

## Implement the `<Login />` component
This basic component should show/hide a login form based your login status. It should be able to communicate with the API server's signin process as well as an OAuth provider.

### Requirements
* Draw a form that takes username and password
* On Submit, issues a `POST` request to the API server's `/signin` route
* Ensure that the server responds properly on a good and bad login
  * A good login should return a header with the token as well as raw text
  * A bad login should return an error from the server
* Implement a link that spawns your OAuth login process
* In both cases, on a good login, set logged in state to `true`
* Implement a Logout link that toggles state
* When logged in, show the logout link and hide the form
* When logged out, hide the logout link and show the form

## Implement the `<LoginContext />` context API Wrapper
This feature will extend the basic login by using the Context API to publish the login state globally.

### Requirements
* Once you have the raw login forms created and working, it's time to use that to persist the users' login status
* Create a provider that publishes into context:
  * Login Status
  * Token Data
  * Login Method
  * Logout Method
* Wrap the application in your `<LoginContext />`
* Marry context and the component, by calling the context's login and logout methods from the login component.
* Take care to add/delete the cookies and manage your state appropriately based on logged in and logged out state.

### Testing
* tests that ensure the list module functions correctly with error-check parameters

##  Documentation
Complete the README.md file included in the lab folder
