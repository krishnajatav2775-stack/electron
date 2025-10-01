#jizfzcxxcxcxvxvxvxcx
xc
xcxx
xx
x
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Message Forward Example</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 20px; }
    #output { margin-top: 20px; padding: 10px; background: #f0f0f0; border: 1px solid #ddd; }
  </style>
</head>
<body>
  <h1>Message Forwarding</h1>
  <label for="message">Enter your message:</label>
  <input type="text" id="message" placeholder="Type your message here" />
  <button id="sendButton">Forward Message</button>

  <div id="output">
    <h3>Forwarded Message:</h3>
    <p id="forwardedMessage">No message yet!</p>
  </div>

  <script>
    // Grabbing elements
    const messageInput = document.getElementById('message');
    const sendButton = document.getElementById('sendButton');
    const forwardedMessage = document.getElementById('forwardedMessage');

    // Event listener for the button
    sendButton.addEventListener('click', () => {
      const message = messageInput.value; // Get the input value
      if (message.trim() !== '') {
        forwardedMessage.textContent = message; // Forward the message
        messageInput.value = ''; // Clear the input field
      } else {

       
