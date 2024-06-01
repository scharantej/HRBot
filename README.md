## Flask Application Design

### HTML Files

**index.html:**
- Home page of the application
- Provides a form to input parameters required for the problem solution
- May include additional sections for displaying results or other information

**results.html:**
- Displays the results of the problem solution
- Uses data passed from the Flask routes to populate the results

### Routes

**@app.route('/')**
- Handles the home page route (index.html)
- May also handle any additional actions on the home page, such as submitting the form

**@app.route('/results')**
- Handles the results page route (results.html)
- Recieves the input parameters from the home page and processes them to generate the solution
- Passes the results data to the results page for display

**@app.route('/other-routes')**
- Additional routes as necessary for the application
- Could handle other functions, such as processing additional user input or accessing external resources