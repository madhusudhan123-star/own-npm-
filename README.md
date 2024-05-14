```
# Basic Request Utilities

This package provides a simple way to import and use the core Node.js modules `http`, `fs`, `path`, and `url`, along with a predefined port number.

## Installation

To install the package, run the following command in your project directory:
```

npm install basic_request_utilities
```
## Usage

1. Import the package in your JavaScript file:

javascript
const { http, fs, path, url, PORT } = require('basic_request_utilities');
```

Use the imported modules and the PORT constant as needed:
```
// Create an HTTP server
const server = http.createServer((req, res) => {
  // Handle requests
});

// Read a file
const fileContent = fs.readFileSync('example.txt', 'utf8');

// Join paths
const filePath = path.join(__dirname, 'data', 'file.txt');

// Parse a URL
const parsedUrl = url.parse('http://example.com/path?query=value');

// Use the predefined PORT constant
server.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
```

Included Modules
  
http: The core Node.js module for creating HTTP servers and clients.
fs: The core Node.js module for working with the file system.
path: The core Node.js module for handling file paths.
url: The core Node.js module for URL resolution and parsing.
PORT: A predefined constant set to 4000, representing the port number to use for your application.

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the package's GitHub repository.  
