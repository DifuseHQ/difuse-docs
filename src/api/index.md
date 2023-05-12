# API

The device offers some API endpoints that you can use for programmatically interacting with it. The below endpoints/lists are in-exhaustive and will be updated as more things get added.

## SMS API

If you have an LTE module in your device, you can use the API to send and receive SMS.

We’re going to assume your LAN IP is 192.168.1.1 in the following examples.

| Route | Function |
| --- | --- |
| `POST /api/sms/get-all` | Get All SMS |
| `POST /api/sms/get-one` | Get Specific SMS using ID |
| `POST /api/sms/delete-one` | Delete specific SMS using ID |
| `POST /api/sms/send-one` | Send an SMS |

The base URL will always be **https://192.168.1.1**, or whatever your LAN IP is (you can also use hostname). The auth parameter for all endpoints is your admin password.

### Getting All SMS

`POST /api/sms/get-all`

This endpoint expects **2** JSON encoded parameters:

```json
{
  "auth": "changemefast",
  "type": "sent" /* or received */
}
```
Here’s an example curl request for getting all Sent and Received SMS:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"auth":"changemefast", "type":"sent"}' https://192.168.1.1/api/sms/get-all -k
```

```bash
curl -X POST -H "Content-Type: application/json" -d '{"auth":"changemefast", "type":"received"}' https://192.168.1.1/api/sms/get-all -k
```

### Getting One SMS

`POST /api/sms/get-one`

This endpoint expects **3** JSON encoded parameters:

```json
{
"auth": "changemefast",
"type": "sent", /* or received */
"id": "1" /* ID of the message */
}
```

### Deleting One SMS

`POST /api/sms/delete-one`

This endpoint expects **3** JSON encoded parameters:

```json
{
"auth": "changemefast",
"type": "sent",
"id": "1"
}
```

Here’s an example curl request for deleting a sent and received SMS:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"auth":"changemefast", "type":"sent", "id": "2"}' https://192.168.1.1/api/sms/delete-one -k
```

```bash
curl -X POST -H "Content-Type: application/json" -d '{"auth":"changemefast", "type":"received", "id": "2"}' https://192.168.1.1/api/sms/delete-one -k
```

### Sending One SMS

`POST /api/sms/send-one`

This endpoint expects **3** JSON encoded parameters:

```
{
"auth": "changemefast",
"to": "123456789", /* number to send sms to */
"message": "<escaped message>"
}
```

Here’s an example curl request for sending an SMS:

```bash
curl -X POST -H "Content-Type: application/json" -d '{"auth":"changemefast", "to":"9078155555", "message":"Hello World!"}' https://192.168.1.1/api/sms/send-one -k
```