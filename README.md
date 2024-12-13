

# Street Smart App


## Table of Contents

- [About](#about)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Demo](#demo)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About

**Street Smart App** is a comprehensive web application designed to enhance local shopping experiences by connecting users with nearby shops and businesses. The app provides detailed shop profiles, user reviews and ratings, product availability filters, and integrated navigation assistance, all presented through a modern and responsive interface.

Developed as part of my internship at **Tech Solutions Pvt. Ltd.**, the Street Smart App aims to bridge the gap between local businesses and consumers, fostering community engagement and supporting small businesses.

## Features

- **Detailed Shop Profiles:** Access comprehensive information about each shop, including location, contact details, operating hours, and available products.
- **User Reviews and Ratings:** Users can rate and review shops based on their experiences, helping others make informed decisions.
- **Product Availability Filters:** Search and filter products based on availability, categories, and other criteria.
- **Navigation Assistance:** Integrated maps and navigation features to help users locate shops easily.
- **Responsive Design:** Ensures seamless user experience across various devices and screen sizes.
- **Secure and Scalable Backend:** Built with Spring Boot and AWS services to ensure high performance and security.

## Technologies Used

- **Frontend:**
  - [Angular](https://angular.io/) - A platform for building mobile and desktop web applications.
  - [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework for rapid UI development.
- **Backend:**
  - [Spring Boot](https://spring.io/projects/spring-boot) - A framework for building production-ready applications in Java.
  - [RESTful APIs](https://restfulapi.net/) - Architectural style for designing networked applications.
- **Database:**
  - [MySQL](https://www.mysql.com/) - An open-source relational database management system.
- **Others:**
  - [Docker](https://www.docker.com/) - Containerization platform for consistent development environments.
  - [Git](https://git-scm.com/) - Version control system for tracking changes.

## Demo

## Installation

### Prerequisites

Before you begin, ensure you have met the following requirements:

- **Node.js** and **npm** installed on your machine. You can download them [here](https://nodejs.org/).
- **Java 11** or higher installed. You can download it from [AdoptOpenJDK](https://adoptopenjdk.net/).
- **Angular CLI** installed globally:

  ```bash
  npm install -g @angular/cli
  ```

- **Maven** installed for backend management. You can download it from [Maven Downloads](https://maven.apache.org/download.cgi).
- **Docker** installed (optional, for containerization).
- An **AWS** account for deploying cloud services (optional, if you plan to deploy).

### Backend Setup

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/deepak170601/street-smart-app.git
    cd street-smart-app/backend
    ```

2. **Configure Environment Variables:**

    Create a `.env` file in the `backend` directory and add the necessary environment variables. Example:

    ```env
    SPRING_DATASOURCE_URL=jdbc:mysql://localhost:3306/streetsmart
    SPRING_DATASOURCE_USERNAME=root
    SPRING_DATASOURCE_PASSWORD=yourpassword
    SPRING_JPA_HIBERNATE_DDL_AUTO=update
    AWS_ACCESS_KEY_ID=your_aws_access_key
    AWS_SECRET_ACCESS_KEY=your_aws_secret_key
    AWS_S3_BUCKET_NAME=your_bucket_name
    ```

3. **Install Dependencies and Build:**

    ```bash
    mvn clean install
    ```

4. **Run the Backend Server:**

    ```bash
    mvn spring-boot:run
    ```

    The backend server should now be running on `http://localhost:8080`.

### Frontend Setup

1. **Navigate to Frontend Directory:**

    ```bash
    cd ../frontend
    ```

2. **Install Dependencies:**

    ```bash
    npm install
    ```

3. **Configure Environment Variables:**

    Create an `environment.ts` file in `src/environments` and add the necessary configuration. Example:

    ```typescript
    export const environment = {
      production: false,
      apiUrl: 'http://localhost:8080/api',
      awsS3Bucket: 'your_bucket_name'
    };
    ```

4. **Run the Frontend Server:**

    ```bash
    ng serve
    ```

    The frontend app should now be running on `http://localhost:4200`.

## Usage

1. **Access the Application:**

    Open your browser and navigate to `http://localhost:4200` to access the Street Smart App.

2. **Register and Login:**

    - Register a new user account.
    - Login with your credentials.

3. **Explore Shops:**

    - Browse through the list of nearby shops.
    - View detailed shop profiles.

4. **User Reviews and Ratings:**

    - Rate and review shops based on your experience.

5. **Product Availability:**

    - Use filters to search for products based on their availability.

6. **Navigation Assistance:**

    - Use the integrated maps to navigate to the selected shop.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. **Fork the Repository**
2. **Create a Feature Branch**

    ```bash
    git checkout -b feature/YourFeature
    ```

3. **Commit Your Changes**

    ```bash
    git commit -m "Add your message"
    ```

4. **Push to the Branch**

    ```bash
    git push origin feature/YourFeature
    ```

5. **Create a Pull Request**

Please ensure your code follows the project's coding standards and passes all tests.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

- **Name:** Chekurthi Deepak
- **Email:** [chekurthideepak@gmail.com](mailto:chekurthideepak@gmail.com)
- **LinkedIn:** [linkedin.com/in/deepak-chekurthi](https://www.linkedin.com/in/deepak-chekurthi-4a10aa202/)
- **GitHub:** [github.com/deepak170601](https://github.com/deepak170601)

---

### **Explanation of the README Sections:**

1. **Project Title & Logo:**
   - Displays the name of the project prominently.
   - Optionally includes a logo for branding.

2. **Table of Contents:**
   - Provides quick navigation to different sections of the README.

3. **About:**
   - Offers a brief overview of what the project is about, its purpose, and its significance.

4. **Features:**
   - Lists the key functionalities and features of the app, highlighting what sets it apart.

5. **Technologies Used:**
   - Enumerates the frameworks, libraries, and tools utilized in developing the application.

6. **Demo:**
   - Showcases a live demo or screenshots/GIFs to provide a visual understanding of the app.
   - Replace the placeholder with actual images or links.

7. **Installation:**
   - **Prerequisites:** Lists the necessary software and tools required to run the application.
   - **Backend Setup:** Step-by-step instructions to set up and run the backend server.
   - **Frontend Setup:** Step-by-step instructions to set up and run the frontend application.

8. **Usage:**
   - Guides users on how to use the application once it's up and running.

9. **Contributing:**
   - Encourages others to contribute to the project and outlines the process to do so.

10. **License:**
    - States the licensing terms under which the project is distributed.

11. **Contact:**
    - Provides contact information for users to reach out with questions or feedback.

### **Additional Recommendations:**

- **Screenshots & Media:**
  - Replace placeholder images (`./assets/logo.png`, `./assets/demo.gif`) with actual screenshots or GIFs of your application to give users a visual representation.

- **Live Demo:**
  - If deployed, provide a live demo link. If not, consider deploying the app on platforms like Heroku, AWS, or GitHub Pages and update the link accordingly.

- **API Documentation:**
  - If your project has extensive API endpoints, consider adding a separate `API.md` or integrating API documentation tools like Swagger.

- **Environment Variables Security:**
  - Ensure that sensitive information like API keys and secrets are not exposed in the repository. Use environment variables and consider adding `.env` files to `.gitignore`.

- **Testing:**
  - Include instructions or details about any tests you've written to ensure the application's reliability.

- **Deployment Instructions:**
  - Provide guidance on how to deploy the application to production environments if applicable.

By following this structure and customizing it with your project's specific details, your `README.md` will effectively communicate the value and functionality of your **Street Smart App** to users and potential contributors.