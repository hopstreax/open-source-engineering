Component

entry.server.tsx

Responsibility

Acts as the entry point for every server-side HTTP request in the Remix application.

Who Calls It?
The Remix/Node.js server when an HTTP request arrives.
Who Does It Call?
handleRequest()
handleBotRequest()
handleBrowserRequest()
renderToPipeableStream()
RemixServer
Responsibilities
Parse the incoming request.
Apply route-specific security headers.
Detect locale.
Detect operating system.
Detect bot vs browser.
Dispatch to the appropriate rendering strategy.
Stream HTML back to the client.
Handle rendering errors.
Key Architectural Decisions
Dispatcher Pattern (handleRequest).
Single Source of Truth (compute locale/platform once).
Streaming SSR.
Separate rendering strategies for bots and browsers.
Timeout protection with abort.
Different error handling before and after streaming starts.
Mental Model

Think of entry.server.tsx as the airport control tower.

Every request lands here first.

The tower:

checks who is arriving,
gathers important information,
decides which runway to use (bot or browser),
then safely guides the response back to the client.
