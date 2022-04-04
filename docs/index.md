# Automated builds CI + CD

CD/CI are methods frequently used to deliver apps to customers making use of automation into the stages of the app development. The main concepts attributed to CD and CI are Continuous Integration for CI and Continuous Delivery and/or Continuous Deployment for CD.
Both methods are quite common into the DevOps world, but what’s DevOps? DevOps is a set of practices that brings together software development (Dev) and IT operations (Ops). Its goal is to make the software development lifecycle faster and provide high quality continuous delivery.
But even though all three are part of the software delivery process, each has its own requirements, and more importantly, benefits. So, understanding the differences between them it’s crucial to properly implementing them.

### CI (Continuous Integration)
Definition

### CI (Continuous Delivery)
Definition

### CI (Continuous Deployment)
Definition

<p>&nbsp;</p>

## How to config automatic builds with GitHub Actions:
After this brief introduction on the pilar concepts about automatic builds, I’ll proceed with the teoric explanation of how to configurate automatic builds using GitHub Actions. But first of all, I would like to explain why you should use this method to create your GitHub builds:
- Avoid having the problems of “It worked on my machine when I built it”.
- Eliminates the human error possibility
- Validate that your builds are running on different platforms.

Now, with that beeing clear we can proceed to cerate a automated build with GitHub actions for the first time. The steps are:
1. First we need to create a repository to be able to configure an automated build.
![](1.jpg)
<p>&nbsp;</p>

2. Go to Actions in the menu above.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/3.jpg)
<p>&nbsp;</p>

3. Create a new worklfow.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/4.jpg)
<p>&nbsp;</p>

4. Set up a workflow yourself.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/5.jpg)
<p>&nbsp;</p>

5. Edit, and when you finish press Start commit.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/6.jpg)
<p>&nbsp;</p>

6. Go back to Actions.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/7.jpg)
<p>&nbsp;</p>

7. Go to the workflow you just created.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/8.jpg)
<p>&nbsp;</p>

8. Run workflow
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/9.jpg)
<p>&nbsp;</p>

9. Check for possible errors.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)

<p>&nbsp;</p>

## Guide to write scripts, manual copying README files, etc:
GitHub Script is an awesome action that allows us to quickly interact with the GitHub API(application programming interface) directly from our workflow. More specifically, we will use the workflow context to script any API that we may need.
To be able to create, add or modify a script we need to return to the .yml file of the workflow where we want the script to be run to.
This means that every time an issue gets opened in this repository the GitHub Script you wrote will execute.

<p>&nbsp;</p>

## Automatically zip and upload back to github (CD):

<p>&nbsp;</p>

## Automatic builds and notifications:
If you enable email or web notifications for GitHub Actions, you'll receive a notification when any workflow runs that you've triggered have completed. The notification will include the workflow run's status (including successful, failed, neutral, and canceled runs). You can also choose to receive a notification only when a workflow run has failed. For more information about enabling or disabling notifications, see "About notifications."
GitHub allows us to change our notification settings and manage our subscriptions. To do that we have to:
1. Click into the bell icon.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
<p>&nbsp;</p>

2. Go to Manage notifications.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
<p>&nbsp;</p>

3. Depending in if you want to change yout notification settings or manage your subscriptions you will chose between Notification settings or Subscriptions.
![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
  <p>&nbsp;</p>
  
  A. Notification settings
  ![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
  
  ![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
  <p>&nbsp;</p>
  
  B. Subscriptions
  ![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
  
  ![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
  
  ![](https://github.com/carlosarnau/Automated-builds-CI-CD/blob/110e4a7eb2f563e968868f8f2aa9284b07df53a1/docs/images/1/10.jpg)
