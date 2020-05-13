# whatsapp_Search_Bot
This is a whatspp searching bot that uses twilio. You just need to send a message with what you're looking for to twilio sandbox in whatsapp and get a reply with the link to the most pertinent result from Google

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

What things you need to install
```
* Node JS
* Visual Studio Code or your favorite IDE
```
### Google Search Engine (GSE) set up
If you already have a GSE account you may want to go to the next section

A step by step instruction that tells you how to get it running

1. Get a  [google search engine API KEY](https://developers.google.com/custom-search/v1/overview) and save it somewhere
2. Create a new project
3. [Set up](https://cse.google.com/cse/all) the custom engine search
4. Use www.google.com as searche engine and save the **Search Engine ID**
5. Go to configuration panel and turn on the **Search the entire web button**

### Twilio Sandbox Set up

1. Create a [Twilio](https://www.twilio.com/) account
2. Create a new project and save the **ACCOUNT SID** and **AUTH TOKEN**
3. Set up the [whatsapp Sandbox](https://www.twilio.com/console/sms/whatsapp/sandbox)

You are now good to go

### Installation

1. Clone this repository
2. Create a .env file in the root directory and add the following information (Replace by your keys and ids)
```
SID = twilio account SID
KEY = twilio account AUTH TOKEN
APIKEY = Google API KEY
CX = GSE Engine ID
```
3.  Install the dependencies
```
npm install
```
4. Run the server
```
npm start
```
5. Run ngrok
```
./ngrok http 3000
```
6. Copy the new server (in this case "https//ffab8079.ngrok,io") and add it to the sandbox![](https://i.imgur.com/lSgs1C4.png) and paste it here 

![](https://i.imgur.com/pjD32Zp.png)

7. Restart your server
Everything is set up and now running! Let do some testing!

### Testing

You can now go to your Whatsapp account and try sending a message to your endpoint.
If everything goes well you should get a response back as shown below !

![](https://i.imgur.com/cuFUUGe.jpg)
