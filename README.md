# GREEN API Test Console

Web interface for testing methods of the GREEN-API service.

This project provides a simple and convenient UI for interacting with the GREEN-API REST API directly from the browser.

It allows sending WhatsApp messages and files as well as checking instance configuration.

---

## Features

- getSettings
- getStateInstance
- sendMessage
- sendFileByUrl

Additional features:

- JSON formatted API responses
- Response copy button
- Response clear button
- Loader during API requests
- Dark / Light theme
- Saving credentials in localStorage

---

## Technologies Used

- HTML5
- CSS3
- Vanilla JavaScript
- Bootstrap 5

External tools:

- GREEN-API
- GitHub Pages (for deployment)

---

## Interface

The interface allows the user to:

1. Enter instance credentials
2. Send WhatsApp messages
3. Send files via URL
4. Retrieve instance settings
5. Retrieve instance state

All API responses are displayed in a formatted JSON field.

---

## API Methods Used

### getSettings

Returns instance settings.


---

### getStateInstance

Returns instance authorization state.

https://api.green-api.com/waInstance%7BidInstance%7D/getSettings/%7BapiTokenInstance%7D



---

### sendMessage

Sends a WhatsApp text message.
https://api.green-api.com/waInstance%7BidInstance%7D/getStateInstance/%7BapiTokenInstance%7D



Example request body:

```json
{
  "chatId": "79999999999@c.us",
  "message": "Hello from API"
}

https://api.green-api.com/waInstance%7BidInstance%7D/sendMessage/%7BapiTokenInstance%7D

POST
https://api.green-api.com/waInstance{idInstance}/sendFileByUrl/{apiTokenInstance}

{
  "chatId": "79999999999@c.us",
  "urlFile": "https://example.com/file.pdf",
  "fileName": "file.pdf"
}


### How to Use
1 Create an instance

Login to GREEN-API console and create a new instance.

Scan the QR code using WhatsApp to connect your phone.