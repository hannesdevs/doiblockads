# Do I Block Ads? 🚫

This is a simple web page that detects if the user is blocking ads using an ad blocker. The page displays the result of the ad blocker status with a corresponding message and icon.

## How it works 🛠️

The code consists of an HTML structure, CSS styles, and JavaScript for the ad blocker detection functionality.

### HTML structure 📄

The HTML structure is minimal, containing a heading, a div for displaying the ad blocker status, and a footer with the author's credit.

### CSS styles 🎨

The CSS styles are included in the `<style>` tag in the `<head>` section. The styles include basic resets, a responsive design with flexbox, and simple animations for displaying the ad blocker status.

### JavaScript functionality 📜

The ad blocker detection functionality is achieved using JavaScript. The `checkAdBlocker()` function creates a script element with a common ad script URL (Google AdSense in this case). It then adds event listeners for the `onerror` and `onload` events of the script element.

- If the ad script fails to load (i.e., it's blocked by an ad blocker), the `onerror` event is triggered, and the status message and styling indicate that ads are being blocked 🚫.
- If the ad script loads successfully (i.e., it's not blocked), the `onload` event is triggered, and the status message and styling indicate that ads are not being blocked ✅.

The `checkAdBlocker()` function is called immediately after its declaration to execute the ad blocker detection process when the web page is loaded.
