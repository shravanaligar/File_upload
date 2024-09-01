# File Upload Page

This project is a simple web application for uploading files, built using Servlet, JSP, Maven, and JDBC. The uploaded files are stored in a specified directory on the server, and their metadata is stored in a database.

## Features

- Upload files through a web interface.
- Store file details (e.g., name, path, upload time) in a database.
- Handle multiple file uploads simultaneously.
- Provide feedback to the user on the success or failure of the upload.

## Technologies Used

- **Servlet**: To handle the file upload request and process the data.
- **JSP**: To create the user interface for file uploading.
- **Maven**: For project management and dependency handling.
- **JDBC**: To interact with the database and store file metadata.


## Setup and Installation

### Prerequisites

- **JDK 8 or higher**: Make sure you have the JDK installed.
- **Maven**: Ensure Maven is installed and configured on your system.
- **Database**: Set up a database (e.g., MySQL) to store the file metadata. Create a table with appropriate columns (e.g., file_name, file_path, upload_time).

### Configuration

1. **Database Configuration**:
   - Update the `DBConnection.java` file with your database URL, username, and password.

2. **Maven Dependencies**:
   - The required dependencies are listed in the `pom.xml` file. These include Servlet API, JSP API, and MySQL JDBC driver. Ensure all dependencies are correctly set up by running:
     ```
     mvn clean install
     ```

3. **Directory Setup**:
   - Create a directory on your server where the uploaded files will be stored. Update the `FileUploadServlet.java` with the path to this directory.

### Running the Project

1. **Build the Project**:
   - Use Maven to build the project:
     ```
     mvn package
     ```

2. **Deploy on Server**:
   - Deploy the generated WAR file to your preferred servlet container (e.g., Apache Tomcat).

3. **Access the Application**:
   - Open your web browser and navigate to:
     ```
     http://localhost:8080/yourproject/upload.jsp
     ```
   - Use the provided form to upload files.

## Usage

1. Open the file upload page in your web browser.
2. Select a file from your local machine.
3. Click "Upload" to submit the file.
4. The file will be stored on the server, and the metadata will be saved in the database.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

- [Servlet API Documentation](https://docs.oracle.com/javaee/7/api/javax/servlet/package-summary.html)
- [JSP Documentation](https://docs.oracle.com/javaee/7/tutorial/servlets012.htm)
- [Maven Documentation](https://maven.apache.org/guides/index.html)
- [JDBC Documentation](https://docs.oracle.com/javase/tutorial/jdbc/)



