**Algorithm to start the Flask application to say "hello world":**

1. **Import Flask**: 
    - `from flask import Flask`
   
2. **Create App Object**:
    - Initialize the Flask class and assign to `app`: `app = Flask(__name__)`
   
3. **Define Route**:
    - Decorate a function with `@app.route('/')`
    - In the function, return `'Hello, World!'`

4. **Run the Application**:
    - Check if the script is executed as the main program: `if __name__ == "__main__":`
    - If true, run the app using: `app.run()`
