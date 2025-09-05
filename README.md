# CompleteFocus---Backend-Part


### Task Tracking & Workflow Management System 

PulseBoard is a modern task tracking and workflow management system designed to help individuals and teams organize tasks, set goals, and monitor progress in real time. It features a dynamic dashboard with a responsive UI, email notifications, and external API integration. Built with Spring Boot, MySQL, AWS on the backend and React + Tailwind CSS on the frontend, PulseBoard is secure, scalable, and user-friendly, making task management simple and efficient.




## API Reference

#### Get all users

```http
  GET /api/users
```

#### Get users by role

```http
  GET /api/users/role/{role}
```

## Goals

#### Create goal

```http
  POST /api/goals
```


#### Get goals by user

```http
  GET /api/goals/user/{userId}
```

#### Close goal

```http
  PUT /api/goals/{goalId}/close
```

## Tasks 

#### Get tasks by user

```http
  GET /api/tasks/user/{userId}

```
#### Mark task complete

```http
  PUT /api/tasks/{taskId}/complete
```
## Reports


#### Get daily report

```http
  GET /api/reports/daily/{userId}?date=YYYY-MM-DD
```

#### Get weekly report

```http
  GET /api/reports/weekly/{userId}
```

#### Get team report

```http
  GET /api/reports/team
```

## Email
### Send report via email


```http
 POST /api/email/send 
```

### Request Params
```http

to → recipient email

subject -> email subject

body -> email body
```

### POST /api/email/send?to=gausul@focus.dev&subject=Daily Report&body=You completed 3 tasks today!


#### add(num1, num2)

Takes two numbers and returns the sum.


## Deployment

To deploy this project run

```bash
  npm run deploy
```

## Deployment

### Prerequisites
- **Java 17+**
- **Maven 3.9+**
- **MySQL 8+**
- (Optional) **AWS Account** if you want to deploy on EC2 or integrate S3
- Git installed

---

### Local Setup

1. **Clone the repository**
```bash
git clone https://github.com/your-username/completefocus.git
cd completefocus


Thanks for reading, let’s build something great together!
