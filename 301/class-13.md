# SENDING FORM DATA

taking data submitted from a form 

## client-server architecture 

- a client (usually a web browser) sends a request to a server 

 - The server answers the request using the same protocol.

 ![d](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)


 > note: An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.


### On the client side: defining how to send the data

The <form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

## action 
The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL.

- The names and values of the non-file form controls are sent to the server as name=value pairs joined with ampersands. The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation. The server then responds, generally handling the data and loading the URL defined by the action attribute, causing a new page load (or a refresh of the existing page, if the action points to the same page).

## method 

The method attribute defines how data is sent.

## Get Method 
 used by the browser to ask the server to send back a given resource

- The data is appended to the URL as a series of name/value pairs. After the URL web address has ended, we include a question mark (?) followed by the name/value pairs, each one separated by an ampersand (&). In this case we are passing two pieces of data to the server


## Post Method 
a method that the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request



- When the form is submitted using the POST method, you get no data appended to the URL, and the HTTP request looks like so, with the data included in the request body instead


