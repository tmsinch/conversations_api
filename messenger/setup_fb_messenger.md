
# Setup an FB App with Messenger Chat
In this quick start guide we will show you how to create and configure a basic FB Business Page with Messenger chat feature.  Once you complete the steps below you will have an FB App, FB Business Page with Messenger Chat button, a Messenger Token, and a configured Messenger Webhook to use with the Sinch Conversations API.


### Sign up for an FB Developer Account or Sign In and Create your Messenger App
To register for an FB Developer account go to **[Facebook Developer Account](https://developers.facebook.com)** and click **"Get Started"** on the upper right menu.

<p align="center">
<img src="./img/fb_for_developers.png" width="75%" border="2px" />
</p>
> 
> If you have an existing FB Developer Account and an FB App, log in and skip to adding and configuring Messenger.
>

Once you have created your Facebook developer account you can choose to **"Create First App"**

<p align="center">
<img src="./img/fb_create_first_app.png" width="35%" border="1" /><img src="./img/fb_create_app_form.png" width="35%" border="1" />
</p>

> 
>Your new *APP ID* will be displayed at the top left of your FB App Dashboard.
>


### Add Messenger Product to your FB App
From your FB Developer Dashboard, under *Add Product*, click on Messenger **"Setup"** button.

<p align="center">
<img src="./img/fb_app_dashboard.png" width="75%" border="1">
</p>


### Create an FB Business Page
Now that you have added Messenger Product to your FB App we can build your first FB Business Page.  Within your Dasboard under Products > Messenger > Settings page scroll down to **Access Tokens** and click **"Create New Page"** on the upper right.

<p align="center">
<img src="./img/fb_create_new_page.png" width="75%" border="1">
</p>

Next choose to create a **"Business or Brand"** and fill out the ensuing page name and contact form.
<p align="center">
<img src="./img/fb_create_business_page.png" width="35%">
<p>
  
You can choose to **"Skip"** adding 'Profile' and 'Background' pictures as well as **"Not Now"** for the option to 'Add online booking'.  You have now completed creating your Facebook Business Page.  Remember while your FB App is 'In development' the FB Business Page is not visible to anyone except you and other developers you invite to your FB developer account.

>
>Make sure to bookmark your FB Business Page , we will return to it later to add a Messenger chat button.
>

<p align="center">
<img src="./img/fb_business_page.png" width="75%">
</p>


### Generate your Messenger API Token
To generate your Messenger API Token we'll need to add the new FB Page you created to the Messenger product settings.  Under Within your Dasboard under Products > Messenger > Settings page scroll down to **Access Tokens** and this type choose to **"Add or Remove Pages"**.

<p align="center">
<img src="./img/fb_add_remove_page.png" width="40%">
</p>

Now follow the prompts and choose the new FB Page you just created.  Make sure that you leave default setting **Manage and access Page converations in Messenger** set to YES.

<p align="center">
<img src="./img/fb_manage_and_access_conversations.png" width="40%">
</p>

You will should see your FB Page listed under **Access Tokens**, click on the **"Generate Token"** button.

>
>Copy and store your Messenger Token somewhere safe, we will need it to add the Messenger Channel to your **Sinch Conversations App**.
>

<p align="center">
<img src="./img/fb_generate_messenger_token.png" width="75%">
</p>


### Add a Messenger Chat Button to your FB Business Page

Lets return to your FB Page and add a Messenger button. Click on **"+ Add Button"** and choose to Send Message.

<p align="center">
<img src="./img/fb_page_add_button.png" width="50%">
</p>
  
Click **"Next"**.
  
  <p align="center">
  <img src="./img/fb_add_send_message_button.png" width="50%">
  </p>
 
 Click on **"Messenger"** and then click **"Finish"**.
 
 <p align="center">
 <img src="./img/fb_add_button_messenger.png" width="50%">
 </p>
 

### Configure the Messenger Webhook

The Messenger Webhook Settings configuration forwards message events posted on your **FB Page** to your **Sinch Conversations App**.  To set the configuration click on **"Add Callback URL"** in FB App Dashboard > Products > Messenger > Settings **Webhooks**.

<p align="center">
<img src="./img/fb_messenger_webhooks.png" width="75%">
</p>

Then add the following **Callback URL** and **Verify Token**:

>
>Callback URL
>https://messenger-adapter.conversation-api.staging.sinch.com/adapter/v1/{{YOUR_SINCH_CONVERSATION_APP_ID}}/callback
>
>Verify Token
>5651d9fd-5c33-4d7a-aa37-5e3e151c2a92
>

<p align="center">
<img src="./img/fb_messenger_edit_webhook.png" width="50%">
</p>

To complete the **Webhook** configuration for Messenger you must click on **"Add Subscriptions"**.

<p align="center">
<img="./img/fp_messenger_webhook_subscriptions.png" width="50%">
</p>





### Configure your FB Messegner Channel on Sinch Conversations API
Steps and images here

### Initiate an FB Messenger Chat and Respond with Sinch Conversations API
Steps and images here

