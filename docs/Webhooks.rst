.. _webhooks:

Webhooks
========

Printdeal API supports webhooks, allowing you to receive real-time notifications about important events. Webhooks are HTTP callbacks triggered when a specific event occurs.

## Base URL

All webhook-related requests start with the following base URL:

```
https://webhook.api.printdeal.com
```

## Managing Webhooks

You can use standard HTTP methods to interact with the webhook API:

### Create a Webhook Subscription

To create a new webhook subscription, send a `POST` request to:

```
POST https://webhook.api.printdeal.com/webhooks
```

Refer to [Creating a subscription](#creating-a-subscription) for more details.

### Retrieve Webhooks

To fetch all your webhooks, send a `GET` request:

```
GET https://webhook.api.printdeal.com/webhooks
```

To retrieve a specific webhook by its UUID, use:

```
GET https://webhook.api.printdeal.com/webhooks/{uuid}
```

Refer to [Retrieving your webhooks](#retrieving-your-webhooks) for more details.

### Delete a Webhook Subscription

To deactivate a webhook, send a `DELETE` request:

```
DELETE https://webhook.api.printdeal.com/webhooks/{uuid}
```

Refer to [Deleting a webhook](#deleting-a-webhook) for more details.

## Testing Webhooks

Before implementing webhooks in your application, you should test them to ensure correct event delivery. You can use webhook testing tools like:

- **[Beeceptor](https://beeceptor.com/)** – Set up a mock endpoint to inspect incoming webhook requests.
- **[Webhook.site](https://webhook.site/)** – Capture and debug webhook payloads in real time.

These tools help you verify the structure and content of webhook requests without writing any code.

---

For more details, visit [Printdeal API Webhooks Documentation](https://docs.api.printdeal.com/docs/Webhooks.html).
