# first-aws-project

DynamoDB CRUD Lambda for managing a contacts list. Built as a first AWS serverless project.

---

## What It Does

A single Lambda function that handles contacts management via an `action` field in the event payload:

| Action | Operation |
|--------|-----------|
| `create` | Add a new contact |
| `update` | Edit an existing contact |
| `get` | Retrieve contacts |
| `delete` | Remove a contact |

---

## Tech Stack

- Python 3
- AWS Lambda
- AWS DynamoDB
- Serverless Framework

---

## Setup

```bash
git clone https://github.com/Hemanth-Py/first-aws-project.git
cd first-aws-project

npm install

sls deploy --stage dev --region us-east-1
```

## Test Locally

```bash
sls invoke local -f lambda_handler --data '{"action": "get"}'
```

---

**Built with:** Python · AWS Lambda · DynamoDB · Serverless Framework
