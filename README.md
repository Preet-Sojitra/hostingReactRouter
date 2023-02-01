# Bug solved:

When hosting serverless web to vercel and when the links are opened in new tab it gives 404 error. To solve this we have to creare `vercel.json` file in root directory. 
This file will redirect to `index.html` file for every route. 
Reason for redirecting to `index.html`: Since react websites are SPAs to all the content will be added in the single `index.html` file, so when we go to `/about` route, its content will be added in `index.html` only. That's why we redirect to `index.html` for all routes
