# File_browser
Simple Fantastic jQuery File Browser



A PHP script - scan.php - scans the Home folder and returns all files and folders as a single JSON object.
Our JavaScript code, with the help of jQuery, takes this JSON, and turns it into a grid of files and folders. Clicking a folder re-renders the view with its contents.
Because there is only one request to the backend involved, browsing through the file list and searching is instantaneous. We also update the URL and use the hashchange event to monitor for navigation using the back/forward buttons.

We invite you to play with the code - it has lots of comments and is relatively easy to follow.

Forcing files to download
Browsers open text files instead of downloading them. If you wish to force all files to download, place this .htaccess file in the files folder:

```
<Files *.*>
ForceType application/octet-stream
</Files>
```

It should be called .htaccess (with a leading dot). This file is only supported on Apache web servers.
