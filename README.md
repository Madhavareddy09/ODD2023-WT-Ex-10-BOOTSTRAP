# Ex-10-BOOTSTRAP
## AIM : To Develop programs to create attractive forms using Bootstrap
## Objective 1 : 
To Create a Responsive feedback form for a virtual workshop on Constructing Modern Websites built with Bootstrap.
## Procedure:
## Step 1:
Identify Form Fields:

Determine the necessary fields such as name, email, and feedback.
## Step 2:
Utilize Bootstrap Components:

Use Bootstrap classes (form-group, form-control, btn) for a responsive and visually appealing form layout.
## Step 3:
Implement Validation:

Add HTML5 validation attributes for required fields and email format.
## Step 4:
Customize Styling:

Adjust the form's appearance using Bootstrap utility classes or custom CSS.
## Step 5:
Test Responsiveness:

Ensure the form is responsive by testing it on various devices.
## Step 6:
Validate Form Submission:

Validate the form data on the server-side to ensure data integrity.

# Program:
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Workshop Feedback Form</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f8f9fa;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        .form-container {
            max-width: 500px;
            background: linear-gradient(to right, #de45d4, #1abc9c);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .form-header {
            text-align: center;
            margin-bottom: 20px;
        }

        label {
            font-weight: bold;
        }

        .form-control {
            border-radius: 5px;
            margin-bottom: 15px;
        }

        button.btn-primary {
            background-color: #007bff;
            border: none;
            width: 100%;
        }

        button.btn-primary:hover {
            background-color: #0056b3;
        }
    </style>
</head>

<body>

    <div class="form-container mt-5">
        <div class="form-header">
            <h2>Workshop Feedback Form</h2>
            <p>We'd love to hear your thoughts!</p>
        </div>
        <form>

            <div class="form-group">
                <label for="fname">First Name:</label>
                <input type="text" class="form-control" id="fname" required>
            </div>

            <div class="form-group">
                <label for="lname">Last Name:</label>
                <input type="text" class="form-control" id="lname" required>
            </div>

            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" class="form-control" id="email" required>
            </div>

            <div class="form-group">
                <label for="number">Phone Number:</label>
                <input type="tel" class="form-control" id="number" required>
            </div>

            <div class="form-group">
                <label for="feedback">Feedback:</label>
                <textarea class="form-control" id="feedback" rows="4" required></textarea>
            </div>

            <div class="form-group">
                <label for="rating">Rating:</label>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="rating" id="rating1" value="5" required>
                    <label class="form-check-label" for="rating1">
                        5 Stars
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="rating" id="rating2" value="4" required>
                    <label class="form-check-label" for="rating2">
                        4 Stars
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="rating" id="rating3" value="3" required>
                    <label class="form-check-label" for="rating3">
                        3 Stars
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="rating" id="rating4" value="2" required>
                    <label class="form-check-label" for="rating4">
                        2 Stars
                    </label>
                </div>
                <div class="form-check">
                    <input class="form-check-input" type="radio" name="rating" id="rating5" value="1" required>
                    <label class="form-check-label" for="rating5">
                        1 Star
                    </label>
                </div>
            </div>

            <button type="submit" class="btn btn-primary">Submit Feedback</button>
        </form>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>

</html>

```
# Output :
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-10-BOOTSTRAP/assets/145742470/c6bbcaa1-5153-48a0-9c2c-29a0de6a7e5f)

# Objective 2 :
To Create a Responsive student registration form for ABC Engineering College built with Bootstrap.

# Procedure :
## Step 1:
Define Form Fields:

Identify fields required for student registration such as name, email, and course selection.
## Step 2:
Use Bootstrap Components:

Utilize Bootstrap form components for a responsive and visually consistent layout.
## Step 3:
Apply Validation:

Implement HTML5 validation attributes for required fields and email format.
## Step 4:
Enhance User Experience:

Improve user experience by using Bootstrap components like dropdowns for course selection.
## Step 5:
Customize Styling:

Customize the form's appearance to align with ABC Engineering College's branding using Bootstrap and custom CSS.
## Step 6:
Test Across Browsers:

Test the form on different browsers to ensure compatibility.

# Program :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f8f9fa;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        .form-container {
            max-width: 600px;
            background: linear-gradient(to right, #6A82FB, #ec8646);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .form-header {
            text-align: center;
            margin-bottom: 20px;
        }

        label {
            font-weight: bold;
        }

        .form-control {
            border-radius: 5px;
            margin-bottom: 15px;
        }

        button.btn-primary {
            background-color: #51ed45;
            border: none;
            width: 100%;
        }

        button.btn-primary:hover {
            background-color: #17d541;
        }
    </style>
</head>

<body>

    <div class="form-container mt-5">
        <div class="form-header">
            <h2>Student Registration Form</h2>
            <p>Welcome to Saveetha Engineering College</p>
        </div>
        <form>

            <div class="form-row">
                <div class="form-group col-md-6">
                    <label for="fname">First Name:</label>
                    <input type="text" class="form-control" id="fname" required>
                </div>
                <div class="form-group col-md-6">
                    <label for="lname">Last Name:</label>
                    <input type="text" class="form-control" id="lname" required>
                </div>
            </div>

            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" class="form-control" id="email" required>
            </div>

            <div class="form-group">
                <label for="phone">Phone Number:</label>
                <input type="tel" class="form-control" id="phone" required>
            </div>

            <div class="form-group">
                <label for="dob">Date of Birth:</label>
                <input type="date" class="form-control" id="dob" required>
            </div>

            <div class="form-group">
                <label for="address">Address:</label>
                <textarea class="form-control" id="address" rows="3" required></textarea>
            </div>

            <div class="form-group">
                <label for="course">Course of Interest:</label>
                <select class="form-control" id="course" required>
                    <option value="" disabled selected>Select Course</option>
                    <option value="computer">Computer Science Engineering</option>
                    <option value="mechanical">Mechanical Engineering</option>
                    <option value="electrical">Electrical Engineering</option>
                    <option value="civil">Civil Engineering</option>
                </select>
            </div>

            <button type="submit" class="btn btn-primary">Submit Registration</button>
        </form>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>

</html>

```
# Output :
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-10-BOOTSTRAP/assets/145742470/1bf31c87-2db4-4da6-9875-6195811c8bf8)
# Objective 3 :
To Develop a program to structure vertical form layouts which handle form validation in bootstrap.

# Procedure :
## Step 1 :
Create HTML Structure:

Design the HTML structure with Bootstrap's form classes for vertical form layout.
## Step 2 :
Leverage Bootstrap Classes:

Use Bootstrap classes (form, form-group, form-control) to create a vertical form layout.
## Step 3 :
Implement Validation Logic:

Write JavaScript code for basic client-side validation, ensuring required fields are filled.
## Step 4:
Add Error Handling:

Provide feedback to users about validation errors using Bootstrap styles.
## Step 5:
Test Across Browsers:

Test the form and validation logic across different browsers.
## Step 6 :
Optimize for Accessibility:

Ensure the form is accessible, adhering to best practices for users with disabilities.

# Program :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vertical Form with Bootstrap Validation</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f8f9fa;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        .form-container {
            max-width: 400px;
            background: linear-gradient(to right, #41e83e, #d839b0);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        label {
            font-weight: bold;
        }

        .form-control {
            border-radius: 5px;
            margin-bottom: 15px;
        }

        button.btn-primary {
            background-color: #007bff;
            border: none;
            width: 100%;
        }

        button.btn-primary:hover {
            background-color: #0056b3;
        }
    </style>
</head>

<body>

    <div class="form-container mt-5">
        <form action="#" method="post" novalidate>
            <div class="form-group">
                <label for="fname">First Name:</label>
                <input type="text" class="form-control" id="fname" name="fname" required>
                <div class="invalid-feedback">
                    Please enter your first name.
                </div>
            </div>

            <div class="form-group">
                <label for="lname">Last Name:</label>
                <input type="text" class="form-control" id="lname" name="lname" required>
                <div class="invalid-feedback">
                    Please enter your last name.
                </div>
            </div>

            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" class="form-control" id="email" name="email" required>
                <div class="invalid-feedback">
                    Please enter a valid email address.
                </div>
            </div>

            <button type="submit" class="btn btn-primary">Submit</button>
        </form>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>

</html>

```
# Output :
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-10-BOOTSTRAP/assets/145742470/6df063aa-084f-4558-b084-41e0e6017509)
# Objective 4 :
To Create a basic email login form in Bootstrap with validation function.

# Procedure :
## Step 1 :
Design Form Elements:

Identify elements needed for an email login form: email input, password input, and submit button.
## Step 2 :
Use Bootstrap Components:

Implement Bootstrap classes (form-group, form-control, btn) for a clean form layout.
## Step 3 :
Incorporate Validation:

Add HTML5 validation attributes and JavaScript code for client-side validation.
## Step 4 :
Apply Styling:

Apply Bootstrap styling for a consistent and visually appealing design.
## Step 5 :
Test Responsiveness:

Ensure the form is responsive by testing it on various devices.
## Step 6 :
Test Login Functionality:

Validate the login form by testing the login functionality on the server side.

# Program :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Email Login Form</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #f8f9fa;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        .form-container {
            max-width: 400px;
            background-color: #ea953f;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        label {
            font-weight: bold;
        }

        .form-control {
            border-radius: 5px;
            margin-bottom: 15px;
        }

        button.btn-primary {
            background-color: #007bff;
            border: none;
            width: 100%;
        }

        button.btn-primary:hover {
            background-color: #0056b3;
        }

        .invalid-feedback {
            display: none;
            color: #dc3545;
            margin-top: 5px;
        }
    </style>
</head>

<body>

    <div class="form-container mt-5">
        <form id="loginForm" action="#" method="post" novalidate>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" class="form-control" id="email" name="email" required>
                <div class="invalid-feedback">
                    Please enter a valid email address.
                </div>
            </div>

            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" class="form-control" id="password" name="password" required>
                <div class="invalid-feedback">
                    Please enter your password.
                </div>
            </div>

            <button type="submit" class="btn btn-primary">Login</button>
        </form>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

    <script>
        // Form validation using JavaScript
        document.getElementById('loginForm').addEventListener('submit', function (event) {
            var isValid = true;

            // Email validation
            var emailInput = document.getElementById('email');
            if (!emailInput.checkValidity()) {
                isValid = false;
                document.querySelector('#email + .invalid-feedback').style.display = 'block';
            } else {
                document.querySelector('#email + .invalid-feedback').style.display = 'none';
            }

            // Password validation
            var passwordInput = document.getElementById('password');
            if (!passwordInput.checkValidity()) {
                isValid = false;
                document.querySelector('#password + .invalid-feedback').style.display = 'block';
            } else {
                document.querySelector('#password + .invalid-feedback').style.display = 'none';
            }

            if (!isValid) {
                event.preventDefault(); // Prevent form submission if validation fails
            }
        });
    </script>

</body>

</html>

```
# Output :
![image](https://github.com/Madhavareddy09/ODD2023-WT-Ex-10-BOOTSTRAP/assets/145742470/42307649-8c57-4966-a08b-d8424bdf19b8)
# Result :
Successfully executed all the given programs using bootstrap.
## Name : K Madhava Reddy
## Register Number : 212223240064
