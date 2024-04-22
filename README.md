# download-pdf-selenium
This project aims to download PDF files using an automation project.

Project Description
Project Title: Selenium Testing Project

Description: This project demonstrates how to automate the download of a PDF file from a web page using Selenium WebDriver with Java and TestNG. The web page contains a link to download a printable PDF cheat sheet. The Selenium script navigates to the web page, locates the download link, and downloads the PDF file to a specified destination folder.

Features
Automates the download of a PDF file from a web page using Selenium WebDriver.
Uses TestNG for test case management and execution.
Configurable destination folder for downloading the PDF file.
Includes a README.md file to provide project information and instructions for usage.

Usage
Clone the repository

Open the project in your preferred IDE.

Please ensure you have installed TestNG, converted the project to it and updated the POM.XML with Selenium and TestNG dependencies. Run the SeleniumTest class as a TestNG test to execute the script.

Rationale Behind Using URLConnection
In this project, i used Java's URLConnection instead of relying solely on Selenium to interact with the browser's UI elements for downloading the PDF file. Here's the rationale behind this approach:

Efficiency: Using URLConnection directly to download files bypasses the overhead of launching a browser instance and interacting with web elements through Selenium. This can result in faster and more efficient downloads.

Simplicity: Working directly with URLConnection simplifies the code and reduces dependencies. There's no need to manage browser sessions, handle browser-specific behaviors, or wait for page loads, which can make the script more robust and easier to maintain.

Resource Management: Selenium is primarily designed for browser automation and testing web applications. While it's capable of downloading files, using it for this purpose may consume unnecessary resources and introduce complexities related to browser automation.

Flexibility: URLConnection provides more flexibility in handling various types of file downloads and interactions with web servers. It allows fine-grained control over HTTP requests and responses, making it suitable for scenarios where precise control is required.

By leveraging URLConnection for file downloads, we can achieve a more lightweight, efficient, and flexible solution compared to relying solely on Selenium for web interactions. This approach complements Selenium's strengths in browser automation while leveraging Java's built-in capabilities for handling network requests.






