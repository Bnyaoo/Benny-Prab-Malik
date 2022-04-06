---
layout: default
title: Troubleshooting guide 
nav_order: 5
---

# Troubleshooting guide 

| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| Unable to load the localhost page | Your URL does not match your port number. | Double check what port you have set in `server.js` and if your browser URL is `localhost:PORT` with `PORT` being the number you have set. |
|ESLint warns you about the use of the console| You have not configured ESLint to accept `console.log`. | Make sure you have `rules: {'no-console': 'off' },` set in `.eslintrc.js` as directed in [Eslint Customization](/pages/configuration/#customization)|
| "TypeError: app.listen is not a function" or similar | You forgot to export one of your modules (ie. app or router). | Make sure you have `module.exports = router;` at the end of your router files and `module.exports = app;` where you created your new Express app.|
| "Error: Cannot find module '<NAME\>'" | You're requiring the module from the wrong path. | Double check the path in the `require(PATH)` is pointing to the correct location.|
| localhost is loading indefinitely | You forgot to include (or you are not hitting) a response method. | Make sure the handler function includes a [response method](/pages/routes#setting-up-routes) to end the HTTP request-response cycle. |
