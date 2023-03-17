# Final Year Project: Foodbank Worker Portal & Admin Portal Repository

This repository contains the code generated by PowerApps for the Foodbank Worker Portal. Currently, PowerApps doesn't support creating a GitHub repository for the Admin Portal, so documentation for the Admin Portal will also be in this document.<br>
This repo is synced to the PowerApps environment so that when the Foodbank Worker Portal is published, changes are committed to this repo.

I have attached the exported solution and the exported TestStudio and I have explained how these can be used in further development below.

## Important Deliverables

Here are all deliverables that I have created as part of this project.<br>
[Repo for Foodbank User Portal on Azure Static WebApps](https://github.com/zcabkle/fyp-foodbank-portal)<br>

[Repo for Foodbank Worker Portal on PowerApps](https://github.com/zcabkle/pa-foodbank-worker-app)<br>

[Exported Solution inc. Foodbank Worker Portal on PowerApps and Admin Portal on PowerApps](https://github.com/zcabkle/pa-foodbank-worker-app/files/10996387/FoodbankSolution_1_0_0_10_managed.zip)<br>
[TestStudio Configuration for Foodbank Worker Portal]()<br>

[Video Overview of the Project](https://www.youtube.com)<br>
[Blog Submission]()<br>

## The Foodbank Worker Portal is currently being hosted.

Access the Foodbank Worker App app via [this access link](https://apps.powerapps.com/play/e/68a17071-5a2a-ea91-a8aa-04cacc480e4e/a/4f0c6aef-95ca-48b9-bf7e-f89cbdc97642?tenantId=f932d2dd-377d-4e9b-bc73-5f0efe92533f) on a laptop or (preferably) on a mobile device with the PowerApps app installed.<br>

The PowerApps app can be found on [Google Play](https://play.google.com/store/apps/details?id=com.microsoft.msapps&hl=en&gl=US) or on the [App Store](https://www.google.com/search?client=safari&rls=en&q=powerapps+app&ie=UTF-8&oe=UTF-8). If the app is installed on your device, when you click the access link you will be asked whether you would like to launch on the PowerApps app, you should click yes.

Use these credentials to login - <br>
Username: <br>
Password: <br>

You should now have access to the Foodbank Worker App on your device.

## The Admin Portal is currently being hosted.

Access the Admin Portal via [this access link](https://org6e7090ee.crm4.dynamics.com/main.aspx?appid=2abc3669-bb8b-4a97-a113-3f7e30a70cf9) on a web browser on a laptop.

Use these credentials to login - <br>
Username: <br>
Password: <br>

## Running Locally

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

Therefore when deploying in PowerApps, assuming users are already part of the current environment, you need to add the user to the app as a 'User' and make sure they have the correct permissions/security role to use the app. An example of an important permission to have is read access to the Dataverse, if users don't have this then they wont be able to view any of the data displayed in the app.

### Steps for Deployment
1. To add a user in the current environment to the app, click the three dot icon and click 'Share'.
2. Find a user with the search bar and assign them an appropriate security role. Fill in the email message if you would like.
![Screenshot 2023-03-17 at 10 59 03](https://user-images.githubusercontent.com/73954803/225886616-e1d27b60-e70b-4404-8311-eac6f74962e7.png)
3. The user will recieve an email with a link to the app. They will also be able to see and access the app whenever they access PowerApps.
4. You can find the access link to the app under 'Details' and 'Web Link' if you ever need to resend a link to a user already added to the app.




