# Email MicroService - Uber Challenge

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)

This project is an email sending RESTful API built using Java, Java Spring and AWS SES.

This NicroService was developed for studies solving the [Uber Challenge](https://github.com/uber-archive/coding-challenge-tools/blob/master/coding_challenge.md).

## Requirements 💻
 To run this project you need to have Java 17 installed on your machine.

 ## Installation 📦

 1. Clone the repository:

```bash
git clone https://github.com/ogabrielalves/email-service.git
```

2. Install dependencies with Maven

3. Update `application.properties` puting your AWS Credentials

```yaml
aws.region=us-east-1
aws.accessKeyId=YOUR_ACCESS_KEY_ID
aws.secretKey=YOUR_KEY_ID
```

## Starting Application 🕹️

1. Start the application with Maven
2. The API will be accessible at http://localhost:8080

## Endpoint 📖

> ### POST Method 🕊️
#### Send a e-mail from your sender to the destination `.../api/email/send`

```json
{
  "to": "lorem@ipsum.com",
  "subject": "Hello World",
  "body": "Hi everyone, this is my first test with AWS SES"
}
```

