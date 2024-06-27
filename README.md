THE APPROACH:

### User Authentication System

A user authentication system is crucial for securing access to applications and services. In this project, we'll create a basic user authentication system using Python, Flask, and SQLite for storing user data securely. We'll also use cryptographic methods to store passwords securely.

### Project Structure :

Here's how our project structure will look:
```
user_authentication/
├── app.py
├── models.py
├── auth.py
├── requirements.txt
└── templates/
    ├── login.html
    └── register.html
```

### Step-by-Step Guide 

#### Step 1: Install Required Libraries

Create a `requirements.txt` file:


flask
flask-sqlalchemy
flask-bcrypt


Install the requirements using pip:
```
pip install -r requirements.txt
```

#### Step 2: Set Up the Flask Application

Create the main application file `app.py`:

```REFER THE CODE AT app.py```

#### Step 3: Define the Database Models

Create a `models.py` file:

```REFER THE CODE AT models.py```

#### Step 4: Implement Authentication Logic

Create an `auth.py` file:

```REFER THE CODE AT auth.py```

#### Step 5: Create HTML Templates

Create a `templates` directory and add `login.html` and `register.html`.

**`login.html`**:

```refer the html code at login.html```

**`register.html`**:

```refer the html code at register.html```

### Explanation

1. **Flask Application (`app.py`)**:
   - Configures Flask application, database, and secret key.
   - Defines routes for user registration, login, dashboard, and logout.
   - Implements session management and user authentication.

2. **Database Models (`models.py`)**:
   - Defines the `User` model with `id`, `username`, and `password` fields.

3. **Authentication Logic (`auth.py`)**:
   - Provides functions for hashing and checking passwords using `bcrypt`.
   - Implements a `login_required` decorator to protect routes.

4. **HTML Templates**:
   - `login.html` and `register.html` provide forms for user login and registration.

### Usage

1. **Set Up the Database**:
   Run the application to create the database and tables:
   ```
   python app.py
   ```

2. **Register a New User**:
   Navigate to `http://127.0.0.1:5000/register` and create a new account.

3. **Log In**:
   Navigate to `http://127.0.0.1:5000/login`, log in with your credentials, and access the dashboard.

4. **Log Out**:
   Click the logout link to end the session.

### Security Considerations

1. **Password Security**:
   - Use `bcrypt` for hashing passwords to ensure they are stored securely.
   - Ensure passwords are not logged or exposed in error messages.

2. **Session Management**:
   - Use secure session management practices, including setting a strong secret key.
   - Implement session timeout and invalidation after logout.

3. **Access Control**:
   - Protect sensitive routes with the `login_required` decorator.
   - Implement role-based access control for more granular permissions.

This project has help me to develop essential skills in user authentication, secure password storage, and access control management, enhancing your cybersecurity profile.

THANK YOU SLASH MARK!
