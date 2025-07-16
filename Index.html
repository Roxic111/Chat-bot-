
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Smart Chatbot</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f0f2f5;
      padding: 40px;
      display: flex;
      justify-content: center;
    }

    .chat-container {
      width: 100%;
      max-width: 600px;
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
      padding: 20px;
    }

    h2 {
      margin-top: 0;
      text-align: center;
      color: #333;
    }

    #chat {
      height: 400px;
      overflow-y: auto;
      border: 1px solid #ddd;
      padding: 15px;
      border-radius: 10px;
      background: #fafafa;
      margin-bottom: 15px;
    }

    .message {
      margin-bottom: 12px;
      padding: 10px 15px;
      border-radius: 10px;
      max-width: 80%;
      line-height: 1.4;
    }

    .user {
      background-color: #dcf8c6;
      align-self: flex-end;
      text-align: right;
      margin-left: auto;
    }

    .bot {
      background-color: #e4e6eb;
      text-align: left;
      margin-right: auto;
    }

    textarea {
      width: 100%;
      padding: 10px;
      font-size: 16px;
      resize: none;
      border-radius: 8px;
      border: 1px solid #ccc;
      box-sizing: border-box;
    }

    button {
      padding: 10px 20px;
      font-size: 16px;
      margin-top: 10px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.2s ease;
    }

    button:hover {
      background-color: #0056b3;
    }

    .examples {
      margin-bottom: 10px;
    }

    .examples button {
      background-color: #e0e0e0;
      color: #333;
      margin: 3px 5px;
      border-radius: 20px;
      font-size: 14px;
      padding: 6px 12px;
    }

    .examples button:hover {
      background-color: #d4d4d4;
    }
  </style>
</head>
<body>
  <div class="chat-container">
    <h2>Smart Chatbot</h2>

    <div id="chat"></div>

    <div class="examples">
      <strong>Try:</strong>
      <button onclick="setQuestion('What is climate change?')">What is climate change?</button>
      <button onclick="setQuestion('Tell me a fun fact')">Tell me a fun fact</button>
      <button onclick="setQuestion('How do airplanes fly?')">How do airplanes fly?</button>
    </div>

    <textarea id="question" rows="3" placeholder="Type your message..."></textarea>
    <button onclick="askQuestion()">Send</button>
  </div>

  <script>
    const apiKey = "place_Api_key_here"; // Replace with your API key

    async function askQuestion() {
      const input = document.getElementById("question");
      const chat = document.getElementById("chat");
      const question = input.value.trim();
      if (!question) return;

      appendMessage(question, "user");
      input.value = "";

      appendMessage("Thinking...", "bot");

      try {
        const response = await fetch("https://api.openai.com/v1/chat/completions", {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            "Authorization": `Bearer ${apiKey}`
          },
          body: JSON.stringify({
            model: "gpt-3.5-turbo",
            messages: [{ role: "user", content: question }]
          })
        });

        const data = await response.json();
        const reply = data.choices?.[0]?.message?.content || "Sorry, no answer found.";
        chat.lastChild.remove(); // Remove "Thinking..."
        appendMessage(reply, "bot");
      } catch (err) {
        chat.lastChild.remove();
        appendMessage("An error occurred. Please check your internet or API key.", "bot");
      }
    }

    function appendMessage(text, type) {
      const chat = document.getElementById("chat");
      const div = document.createElement("div");
      div.className = "message " + type;
      div.innerText = text;
      chat.appendChild(div);
      chat.scrollTop = chat.scrollHeight;
    }

    function setQuestion(text) {
      document.getElementById("question").value = text;
      askQuestion();
    }

    window.onload = () => {
      appendMessage("Welcome! Ask me anything or try one of the example questions below.", "bot");
    };
  </script>
</body>
</html>
