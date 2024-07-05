# some-console-script
**script:Remove friend sent request in facebook.com**
You can easily cancel sent friend requests on Facebook without using third-party applications or extensions. Follow these simple steps:

**Step 1**: Go to the Facebook Friend Requests Page
Visit the following link: https://www.facebook.com/friends/requests/

**Step 2**: Inspect the Page or F12 to open Dev-tools console menu
Right-click on the page and choose "Inspect" from the options menu, or simply press F12 to open the browser's developer tools.

**Step 3**: Click to View sent requests hyperlinks
Now Hold you Left-mouse button to see it scrolling to the top down list you want to cancel

**Step 4**: Execute the JavaScript Code
Copy and paste the following JavaScript code into the console and press Enter:
```javascript
// Get all elements with the aria-label "Cancel request" and role "button"
var cancelButtons = document.querySelectorAll('[aria-label="Cancel request"][role="button"]');

// Loop through and click each button
cancelButtons.forEach(function(button) {
    button.click();
});
```
