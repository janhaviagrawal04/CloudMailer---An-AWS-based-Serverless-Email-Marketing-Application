# 📧 Serverless Email Marketing Application

This project is a hands-on tutorial demonstrating how to design and build a simple serverless email marketing application using AWS services. The application sends emails on a schedule, pulling HTML email templates and a list of contacts from an S3 bucket.

## 🛠️ AWS Services Used

- **📤 Simple Email Service (SES):** To send emails.
- **⏰ EventBridge:** To schedule email sending.
- **📦 S3:** To store email templates and contact lists.
- **📝 Lambda:** To handle the logic for sending emails.
- **🔒 Identity & Access Management (IAM):** To manage permissions and roles.

## 📝 Prerequisites

- **📧 Email Addresses:** You need email addresses that you can validate (both sender and receiver).
- **🌐 Domain:** The sender's email address must be from your own domain.
- **🧠 Basic AWS Knowledge:** Familiarity with AWS services and the AWS Management Console.
- **🖊️ Text Editor:** To write or edit HTML code for the email templates.

## 🚀 Getting Started

### Step 1: Set Up S3 Bucket
1. Create an S3 bucket to store your HTML email templates and contact list.
2. Upload the provided `email_template.html` and `contacts.csv` to your S3 bucket.

### Step 2: Configure Amazon SES
1. Set up Amazon SES with your domain and validate email addresses.
2. Move SES out of the sandbox environment to remove limitations.

### Step 3: Develop Lambda Function
1. Create a Python Lambda function that retrieves the email template and contact list from S3, personalizes the emails, and sends them via SES.
2. 🧪 Test your Lambda function to ensure it works correctly.
3. Update the Lambda execution role with the necessary permissions for S3 and SES.

### Step 4: Schedule Email Sending with EventBridge
1. Create an EventBridge rule to trigger your Lambda function on a schedule.
2. 🧪 Test the EventBridge schedule to ensure emails are sent as expected.

### Step 5: 🧹 Cleanup
1. After testing, make sure to delete all AWS resources (S3 bucket, SES configurations, Lambda functions, EventBridge rules) to avoid incurring unnecessary charges.

## 📂 Resources

- **[📄 Email Template]**
- **[📄 Contacts List]**
- **[📄 Lambda Code and Policies]**

## 💡 Enhancements

Here are a few ideas to extend the functionality of this application:
- Add support for multiple email templates.
- Implement a retry mechanism for failed emails.
- Integrate with a database like DynamoDB to store campaign results.

## ⚠️ Important Notes

- **💰 Costs:** Running this application on AWS may incur costs, depending on your usage.
- **🔑 Permissions:** Ensure you properly configure IAM roles and policies to avoid permission errors.

## 🔗 Related Projects

- [AWS Project: Architect and Build an Email System Using DynamoDB, API Gateway, and Lambda](#)

## 🙌 Credits

This project is inspired by a tutorial created by [Your Name](#).
