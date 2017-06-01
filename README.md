# Using Google Assistant to tell facts about Google using api.ai

This is a knowledgable Assistant app that shares interesting facts about Google.
The sample introduces advanced features like custom entities, contexts,
and deep links. 

## Setup Instructions

See the developer guide and release notes at [https://developers.google.com/actions/](https://developers.google.com/actions/) for more details.

### Steps
1. Use the [Actions on Google Console](https://console.actions.google.com) to add a new project with a name of your choosing.
1. Click "Use API.AI" and then "Create Actions on API.AI".
1. Click "Save" to save the project.
1. Click on the gear icon to see the project settings.
1. Select "Export and Import".
1. Select "Restore from zip". Follow the directions to restore from the FactsAboutGoogle.zip in this repo.
1. Deploy the fulfillment webhook to your preferred hosting environment
(we recommend [Google Cloud Functions](https://cloud.google.com/functions/docs/tutorials/http)).
1. In the Fulfillment page of the API.AI console, enable Webhook, set the URL to the hosting URL, then save.
1. In the quit_facts intent, check "End Conversation" for Actions on Google.
1. Open API.AI's Integrations page, open the Settings menu for Actions on Google.
1. Enter the following intents as "Additional triggering intents"
    * choose_fact
    * choose_cats
1. Click Test.
1. Click View to open the Actions on Google simulator.
1. Type "Talk to my test app" in the simulator, or say "OK Google, talk to my test app" to any Actions on Google enabled device signed into your developer account.

