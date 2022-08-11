# Juicebox-Grading-Tool

## Steps
1. Import `endpointsToGrade.json` into Thunder Client as a collection
1. Add a `JWT_SECRET` variable to `.env`
2. Run the login endpoint to generate a token
3. Add the token as a local environemnt to Thunder Client
4. Select "Run All" in the Juicebox Grading collection menu

## Feedback templates
* All pass: "Great job with this project! Everything is working well and the code is clean. If you have any questions with the feedback or any of the material feel free to reach out over slack or schedule office hours."
* /api/users/login bad credentials returns a 200 status code: "Your error handler does not change the res.status code. For example, the server responds with status 200 even if someone attempts to login with bad credentials. When you pass an error to next(), make sure you change the res.status code at some point before res.send is called."
* missing an else block after `if (id)` in /api/index.js: "Line X has an if (id) block, without an else block which will cause the request to time out if the id is missing from the token."
