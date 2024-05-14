# My Flask App

This is a simple Flask application that displays a "Hello, World!" message.

## Project Structure

```
my-flask-app
├── app
│   ├── __init__.py
│   └── routes.py
├── Dockerfile
├── Jenkinsfile
├── requirements.txt
└── README.md
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/my-flask-app.git
   ```

2. Change into the project directory:

   ```bash
   cd my-flask-app
   ```

3. Create a virtual environment:

   ```bash
   python3 -m venv venv
   ```

4. Activate the virtual environment:

   - For Windows:

     ```bash
     venv\Scripts\activate
     ```

   - For macOS and Linux:

     ```bash
     source venv/bin/activate
     ```

5. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Start the Flask development server:

   ```bash
   flask run
   ```

2. Open your web browser and visit `http://localhost:5000` to see the "Hello, World!" message.

## Docker

To run the Flask application using Docker, follow these steps:

1. Build the Docker image:

   ```bash
   docker build -t my-flask-app .
   ```

2. Run the Docker container:

   ```bash
   docker run -p 5000:5000 my-flask-app
   ```

3. Open your web browser and visit `http://localhost:5000` to see the "Hello, World!" message.

## Jenkins

The Jenkins pipeline for this project is defined in the `Jenkinsfile`. It includes the following stages:

1. Checkout: This stage checks out the source code from the repository.

2. Build: This stage builds the Docker image for the Flask application.

3. Deploy: This stage deploys the Docker container to the desired environment.

Please configure your Jenkins pipeline according to your specific requirements.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvement, please feel free to create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).