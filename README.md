# DialogFlowChatBot1

## Features:

1. -p, --parser - Like a user and retrieve their ID
2. -d, --downloads - Retrieve a list of all Instagram and VK accounts from previously obtained IDs
3. -c, --chat - Chat with the bot


## Installation:

1. You need to register with a phone number on Tinder.com
2. Setting up AI
    First, go and register on Dialogflow (just log in using your Google account). Immediately after authorization, we land on the control panel.
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/fc9/02e/4f6/fc902e4f678af02b0ee1661c521a492d.png)
    
    Click on the Create agent button and fill in the fields as you see fit (this will not play any role, it's just for the next action).
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/91d/5a7/13b/91d5a713b50ccbccc1e4481a6796a008.png)
    
    Click on Create and see the following picture:
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/481/d0f/e72/481d0fe726ec808276a55d5e578ec076.png)
    
    I'll tell you why the "Agent" we created earlier does not play any role. In the Intents tab, there are "commands" that the bot works with. Currently, it can only respond to phrases like "Hello", and if it doesn't understand, it responds with "I did not understand you". Not very impressive.
    After creating our empty agent, we got a bunch of other tabs. We need to click on Prebuilt Agents (these are specially trained agents that have many commands) and from the entire list presented select Small Talk.
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/cee/bd1/f38/ceebd1f3821538f2f690381e7a23cb70.png)
    
    Hover over it and click Import. Then, without changing anything, click Ok. The agent has been imported and now we can configure it. For this, in the upper left corner, click on the gear next to Small-Talk and we get to the settings page. Now we can change the name of the agent as we want (I leave it as it was). Change the timezone and in the Languages tab, check that Russian language is set (if not, then set it).
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/00a/a69/4c0/00aa694c086df5e6a45fd3adc33cc37a.png)
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/2a5/b6f/9c0/2a5b6f9c01de1642f85576adadc555c4.png)
    
    Return to the General tab, scroll down a bit and copy the Client access token
    
    ![alt tag](https://habrastorage.org/getpro/habr/post_images/9c9/496/61c/9c949661c0babb224108df581a782994.png)
    
    Now our AI is fully configured, you can go back to the bot.
3. In the *main.py* script, insert the previously obtained *Client access token* at line 16. The program is ready to run.


## How to use:
```bash
python main.py -h
