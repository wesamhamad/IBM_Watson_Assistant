# Enhance the user experience by Building a chatbots with IBM Watson Assistant
In this code pattern, we walk you through a working example of a web page (ROBOT CONTROL) that utilizes  Watson services to create a better customer care experience.
By using Watson Assistant, we will give customers the answers they need quickly, easily and across any channel. 

## What is IBM Watson Assistant ?
 IBM Watson® Assistant is a question-and-answer system that provides a dialog with fast, consistent and accurate answers to interaction between the conversation system and users across any messaging platform, application, device or channel. Using artificial intelligence and natural language processing, Watson Assistant learns from customer conversations  . This style of interaction is commonly called a chatbot.

## What is a chatbot?
A chatbot is a support system for your customer service. Using artificial intelligence and natural language processing, your chatbot can simulate conversation with a user through messaging applications, websites, mobile apps and more, giving them accurate and relevant information. By powering your chatbot with Watson Assistant, you can avoid the difficulties associated with traditional bots and build a tool that will improve your customer support.

![image](https://user-images.githubusercontent.com/74800962/124354823-ab85dc80-dc16-11eb-9f59-eeac82b211e4.png)




## Chatbot tutorial 
Take a short tutorial of IBM Watson Assistant chatbot technology. You'll create intents and entities and learn how to structure your chatbot conversational flow.
[Step-by-step tutorial](https://cloud.ibm.com/docs/assistant?topic=assistant-getting-started) .

# " Fango " my IBM Watson Assistant (Output Samples)


* Tablets view

https://user-images.githubusercontent.com/74800962/124358745-5784f300-dc2a-11eb-9d14-f20aee35eba8.mov


* Desk top view

https://user-images.githubusercontent.com/74800962/124358551-82bb1280-dc29-11eb-97f7-5a43e0ecc849.mov


## Fango's Dialogs  
* Intents (8)
* Entity (2)
 
![Screen Shot 1442-11-23 at 6 21 03 PM](https://user-images.githubusercontent.com/74800962/124359072-fcec9680-dc2b-11eb-91e5-9807229c295d.jpg)
```
NOTE:
I add child node and customized it as Multipule responses (If you enable multiple responses then your bot can provide different responses to the same input, based on other conditions ), then I made the parent node jump to child node when the condition is met.
```
![n](https://user-images.githubusercontent.com/74800962/124359168-7be1cf00-dc2c-11eb-9b89-3e4926e4a7ca.jpg)

![Screen Shot 1442-11-23 at 6 21 20 PM](https://user-images.githubusercontent.com/74800962/124359076-0118b400-dc2c-11eb-9962-56853cedf00d.jpg)

## </> Embed on my website
After I have finished build a web chat integration, the Watson Assistant UI gives me a small embed code to add it to my website.
```javascript
<script>
  window.watsonAssistantChatOptions = {
      integrationID: "45fc2050-7955-43c3-9957-35fc21c27d85", // The ID of this integration.
      region: "eu-gb", // The region your integration is hosted in.
      serviceInstanceID: "b7623134-fcde-4d2a-811b-a586272aadcc", // The ID of your service instance.
      onLoad: function(instance) { instance.render(); }
    };
  setTimeout(function(){
    const t=document.createElement('script');
    t.src="https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
    document.head.appendChild(t);
  });
</script>
```
## View the chatbot as a [json file](https://github.com/wesamhamad/IBM_Waston_Assistant/blob/main/skill-Fango.json)
## You can try [my chatbot](https://web-chat.global.assistant.watson.cloud.ibm.com/preview.html?region=eu-gb&integrationID=bd3a93c1-cf1b-41d9-96df-49e004bf46be&serviceInstanceID=b7623134-fcde-4d2a-811b-a586272aadcc) 
