### Python code to connect to an SQLite3 database and print a success message upon a successful connection:

```python
import sqlite3

# Connect to the database (or create it if it doesn't exist)
conn = sqlite3.connect('mydatabase.db')

# Check if the connection was successful
if conn:
    print("Connected to the database successfully!")
    
# Don't forget to close the connection when done
conn.close()
```

When you run this script, if there are no errors, it'll connect to the SQLite3 database (or create a new one named `mydatabase.db` if it doesn't already exist) and print the success message. Always remember to close the connection when you're finished with it to free up resources.
