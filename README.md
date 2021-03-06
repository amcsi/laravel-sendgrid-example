# Laravel SendGrid Example

## Etc

### Command

`php artisan io:email-test --to=<address>`

You can add multiple `--to=<address>` arguments to send to multiple email addresses. You can test sending to multiple users with different names to see different "Dear {{name}}," placeholders replaced.

### Env vars

```dotenv
SENDGRID_API_KEY=
SENDGRID_UNSUBSCRIBE_GROUP_ID=
SENDGRID_TEMPLATE_ID=
```

### Template

The template file used is:
`app/Console/Commands/EmailSendTestCommand/template.html`.

This file is not directly used in this project; rather it is (to be) kept in sync with the template used within the SendGrid account and referenced by template ID.
