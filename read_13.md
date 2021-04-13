# Sending form data
## Client/server architecture

![c](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)

At it's most basic, the web uses a client/server archituecture that can be summarized :
1. A web browser sends a reqest to a server
2. The server responds and sends the data back

## Send the data
A `<form>` element defines how the data will be sent. All of it'ts attributes are designed to let you configure a request to be sent when the user hits a submit button. Two important attributes are __action__ and __method__.

The __action__ attribute defines where the data will be sent. The value must be a valid relative or absolute URL. If this is not provided, data will not be sent to the URL of the page containing the form

Example HTML:

`<form action="https://example.com">`

The __method__ attribute defines how data is sent. A HTTP protocol provides several ways to perform requests, HTML form data can be transmitted via a number of different methods, the most common being __Get__ and __Post__.

### GET method

method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.

### POST method

It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

## Viewing HTTP requests
1. Open the developer tools.
2. Select "Network"
3. Select "All"
4. Select `"foo.com"` in the "Name" tab
5. Select "Headers"

![i](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/network-monitor.png)

