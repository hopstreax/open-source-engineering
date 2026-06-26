Component: handleRequest()
Responsibility

Acts as the main request dispatcher.

Responsibilities Verified So Far
Reads information from the incoming request.
Parses the URL.
Applies route-specific security headers.
Determines the user's preferred language.
Detects the user's operating system.
Determines whether the client is a bot or a browser.
Dispatches the request to the appropriate handler.
Mental Model

Imagine an airport security checkpoint.

Every passenger passes through the same entrance.

The checkpoint asks:

Which flight?
Passport?
Special handling?
Domestic or international?

Then it sends the passenger to the correct gate.

handleRequest() does the same thing for HTTP requests.
