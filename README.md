# Final Year Project: Foodbank Worker Portal & Admin Portal Repository

This repository contains the code generated by PowerApps for the Foodbank Worker Portal. <br>

Currently, PowerApps doesn't support creating a GitHub repository for the Admin Portal, so documentation for the Admin Portal will also be in this document. The Admin Portal is included in the solution file provided in this README.md <br>

This repo is synced to the PowerApps environment so that when the Foodbank Worker Portal is published on my environment, changes are committed to this repo. You can set this up by yourself once you have set up this project for local development by following [this guide](https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/git-version-control).

I have attached the exported solution and the exported Test Studio and I have explained how these can be used in further development below.

## Important Deliverables

Here are all deliverables that I have created as part of this project.<br>
[Repo for Foodbank User Portal on Azure Static WebApps](https://github.com/zcabkle/fyp-foodbank-portal)<br>

[Repo for Foodbank Worker Portal on PowerApps](https://github.com/zcabkle/pa-foodbank-worker-app)<br>

[Exported Solution inc. Foodbank Worker Portal on PowerApps and Admin Portal on PowerApps](https://github.com/zcabkle/pa-foodbank-worker-app/files/10996387/FoodbankSolution_1_0_0_10_managed.zip)<br>
[TestStudio Configuration for Foodbank Worker Portal](https://github.com/zcabkle/pa-foodbank-worker-app/files/11002112/Automated.Integration.Tests.fx.yaml.zip)<br>

[Video Overview of the Project](https://www.youtube.com)<br>
[Blog Submission]()<br>

## The Foodbank Worker Portal is currently being hosted.

1. Access the Foodbank Worker App app via [this access link](https://apps.powerapps.com/play/e/68a17071-5a2a-ea91-a8aa-04cacc480e4e/a/4f0c6aef-95ca-48b9-bf7e-f89cbdc97642?tenantId=f932d2dd-377d-4e9b-bc73-5f0efe92533f) on a laptop or (preferably) on a mobile device with the PowerApps app installed.<br>

2. The PowerApps app can be found on [Google Play](https://play.google.com/store/apps/details?id=com.microsoft.msapps&hl=en&gl=US) or on the [App Store](https://www.google.com/search?client=safari&rls=en&q=powerapps+app&ie=UTF-8&oe=UTF-8). If the app is installed on your device, when you click the access link you will be asked whether you would like to launch on the PowerApps app, you should click yes.

3. 
Use these credentials to login - <br>
Username: AlexW@7nqjjm.onmicrosoft.com
Password: <br>

Or

Use these credentials to login - <br>
Username: AdeleV@7nqjjm.onmicrosoft.com
Password: <br>

**(Alex has access to 3/3 foodbanks, Adele only has access to 2/3 foodbanks).**

5. **You may be asked to enter use an authenticator code, refreshing the age removes this prompt.**<br>
6. **You may be asked to extend your PowerApps plan, please select yes if this prompt appears, fill out the other information apart from the phone number.**
7. **You may be required to allow perimission for the connectors. Allow permission for the connectors on this screen**<br>
<img width="512" alt="image" src="https://user-images.githubusercontent.com/73954803/226182879-1ce184b0-73a2-4ff6-9205-c16c2adf6c26.png">

You should now have access to the Foodbank Worker App on your device.

## The Admin Portal is currently being hosted.

Access the Admin Portal via [this access link](https://org6e7090ee.crm4.dynamics.com/main.aspx?appid=2abc3669-bb8b-4a97-a113-3f7e30a70cf9) on a web browser on a laptop.

Use these credentials to login - <br>
Username: LeeG@7nqjjm.onmicrosoft.com
Password: <br>

## Running Locally

### Side Notes

Both the 'Foodbank Worker Portal' and the 'Admin Portal' parts of the project are under the same solution. By setting up the .zip file for running locally, you will set up both portals in one set of steps!

### Steps to Run Locally

1. If you don't already have a Microsoft Developer account, create one here https://developer.microsoft.com/en-us/microsoft-365/dev-program .<br>
2. Download the .zip file via the "Exported Solution inc. Foodbank Worker Portal on PowerApps and Admin Portal on PowerApps" link in the "Important Deliverables" section.
3. Login to PowerApps, on the top-right corner you should be in the environment that has your name, if not click the current environment to change environment to the one with your name (you want to be in this environment as it is a developer environment).![image](https://user-images.githubusercontent.com/73954803/225882057-d8f40081-07d9-4f8a-90c5-b6c76da6fdfd.png)
4. Navigate to solutions via the sidebar menu.<br>
![Screenshot 2023-03-17 at 10 42 07](https://user-images.githubusercontent.com/73954803/225882966-a7c2b95d-cc55-476d-846e-c08dcc816c53.png)
5. Choose to import a solution on the top-bar, and upload the .zip file that you downloaded in step 2. Fill any necessary information and make your way through any prompts.
6. The solution will be available in your solutions menu now. Click into the 'Foodbank Solution' to see all of the objects that are part of the solution.
7. You will now be able to run the 'Admin Application' and 'Foodbank Worker App' by clicking into them from the solutions menu. 
![Screenshot 2023-03-17 at 10 49 58](https://user-images.githubusercontent.com/73954803/225884735-d3aa4925-979b-4cde-a248-67354dbf5647.png)

Click the three dots next the any object and click edit to edit them. This is how you should further develop this project.

## Deployment

### Side Notes
Each time you publish changes to an application on an environment, the changes are accessible to anyone who has been added as a 'User' to the app on that same environment.<br>

Therefore when deploying in PowerApps, assuming users are already part of the current environment, you just need to add the user to the app as a 'User' and make sure they have the correct permissions/security role to use the app. An example of an important permission to have is read access to the Dataverse, if users don't have this then they wont be able to view any of the data displayed in the app!

### Steps for Deployment

**Follow all of the the steps to run locally before trying to deploy**

1. To add a user in the current environment to the app, click the three dot icon and click 'Share'.
2. Find a user with the search bar and assign them an appropriate security role. Fill in the email message if you would like.
![Screenshot 2023-03-17 at 10 59 03](https://user-images.githubusercontent.com/73954803/225886616-e1d27b60-e70b-4404-8311-eac6f74962e7.png)
3. The user will recieve an email with a link to the app. They will also be able to see and access the app whenever they access PowerApps.
4. You can find the access link to the app under 'Details' and 'Web Link' if you ever need to resend a link to a user already added to the app.

## Testing

### Side Notes

Testing is done with the [PowerApps Test Studio](https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/test-studio) which only supports testing on canvas apps.

**Currently, Microsoft documentation doesn't explain how to upload a downloaded test suite in order to run the tests though I have included this testing configuration in the 'Important Deliverables' section for if they implement this in the future.**

### Running the Test Studio

*Until Microsoft implement a feature for uploading a test suite this is a temporary way to get around it. I recommend writing your own tests from scratch or skipping this step entirely.

Prerequisites - 
  Download the 'TestStudio Configuration for Foodbank Worker Portal' given in the 'Important Deliverables' section
  Follow the steps to set up the project to run locally.
  Testing in a separate environment to the one you develop in is highly recommended. Learn how to create a new environment [here](https://learn.microsoft.com/en-us/power-platform/admin/create-environment)
  
1. Go into your solution, click the three button icon and click edit.<br>
2. Navigate to the Test Studio via this menu.<br>
<img width="1440" alt="Screenshot 2023-03-17 at 15 17 54" src="https://user-images.githubusercontent.com/73954803/225946716-e6cd04ef-589d-47de-a788-9bf67e7df37f.png">
3. Open the TestStudio configuration in an IDE such as VSCode.<br>
4. The configuration shows the steps that I used in each test case.<br>
5. For each test case in the configuration, create one on Test Studio and fill in the test steps with the content provided in the configuration file.<br>

## Useful Documentation & Resources

[How to add users to a PowerApps Environment](https://learn.microsoft.com/en-us/power-platform/admin/add-users-to-environment)<br>
[How to configure security roles](https://learn.microsoft.com/en-us/power-platform/admin/database-security)
[PowerPlatform Admin Documentation](https://learn.microsoft.com/en-us/power-platform/admin/)<br>
[PowerApps Learn](https://learn.microsoft.com/en-us/training/powerplatform/power-apps)<br>
[PowerApps Test Studio](https://learn.microsoft.com/en-us/power-apps/maker/canvas-apps/test-studio)
