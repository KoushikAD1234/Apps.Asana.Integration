# Asana Integration for Rocket.Chat


The Asana App for Rocket.Chat  provides a seamless integration between Asana and Rocket.Chat and improves collaboration between teams.
The application allows users to create and manage thier tasks and workspace, subscribe to task events, create new tasks, edit and delete their tasks, attachments, projects & workspaces and do much more right from Rocket.Chat.


<h2>🚀 Features </h2>
<ul>
  <li>Quick and easy setup.</li> 
  <li>Login to Asana with one click using built-in OAuth2 mechanism.</li>
  <li>Subscribe to Task Events and get notified about new comments, priority changes, assignee updates, etc.</li>
  <li>Retreive and manage tasks right from Rocket.Chat channels.</li>
  <li>Create new tasks from Rocket.Chat and make channel of task assignees.</li>
  <li>Edit the tasks right in Rocket.Chat and share them with other channel members.</li>
</ul>


<h2>🔧 Installation steps </h2>

 1. Clone this repo and Change Directory: </br>
 `git clone https://github.com/RocketChat/Apps.Asana.Integration.git && cd Apps.Asana.Integration/`

 2. Install the required packages from `package.json`: </br>
	 `npm install`

 3. Deploy Rocket.Chat app:
 `rc-apps deploy --url <deployment_url> --username <user_username> --password <user_password>`
Where:
- `<deployment_url>` is your local server URL (if you are running in another port, change the 3000 to the appropriate port)
- `<user_username>` is the username of your admin user.
- `<user_password>` is the password of your admin user.

For more info refer [this](https://developer.rocket.chat/apps-engine/getting-started/rocket.chat-app-engine-cli) guide.

<h2>📲 Setup guide </h2>
 <ul>
  <li> You must first register your application with Asana to receive a client ID and client secret by following these steps: [Asana App Registration Guide](https://developers.asana.com/docs/oauth#register-an-application)</li> 
  
  
  <li>Fill the details in the Asana app on your Rocket Chat server by following these steps:</li>
  
  1. Navigate to Administration->Apps. 
  
  2. Select the Installed tab.
  
  3. Click on Asana, and go to Settings tab.
  
  4. Enter your generated a Client ID and Client Secret and click on Save changes button.
  
  <li>Start the authorization by using /asana-app auth slash command.</li>
</ul>


