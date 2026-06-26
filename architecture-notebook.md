Component: handleRequest()

Responsibility (Current Hypothesis)

Acts as the main dispatcher for incoming HTTP requests.

Inputs

Incoming HTTP request
Response status
Response headers
Remix rendering context

Likely Outputs

A rendered HTTP response

Mental Model

Think of handleRequest() as an airport traffic controller.

Every incoming plane (request) contacts the control tower first.

The tower doesn't fly the plane.

It decides where it should go next.

Some requests go to the browser handler.

Some requests go to the bot handler.
