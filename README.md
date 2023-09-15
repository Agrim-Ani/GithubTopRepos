# GithubTopRepos
Scriptable widget that shows top 5 GitHub repos related to the topic


# iOS Scriptable Widget with GitHub Repo Spotlight

This project demonstrates how to create an iOS Scriptable widget that displays the top GitHub repositories based on a topic of your choice. Users can input the desired topic using an iOS Shortcuts automation, and the widget will dynamically update with the top repositories for that topic.

## Overview

- **Scriptable**: Scriptable is an iOS app that allows you to create JavaScript widgets and automations. In this project, we use Scriptable to create a widget that fetches data from GitHub's API and displays it on your iOS home screen.

- **iOS Shortcuts**: We use iOS Shortcuts to gather user input (the GitHub topic) and store it in iCloud for the widget to access.

## Prerequisites

- **Scriptable App**: You need to have the Scriptable app installed on your iOS device. You can download it from the App Store.

## How to Use

1. **Set Up iOS Shortcut**:
   - Create a new iOS Shortcut.
   - Add an action to set a variable. Name it `widgetParameter` and set its value to the GitHub topic you want to spotlight.
   - Add an action to run the Scriptable script with the `widgetParameter` as an input.
   - Create the shortcut as shown in image
   - ![image 1](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/1.PNG)
   - Write the shortcut-script.js in the scriptable app action
   - ![image 2](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/2.jpg)

2. **Run iOS Shortcut**:
   - Add the shortcut to ios homescreen.
   - ![image 3](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/3.jpg)
   - Run the iOS Shortcut you created, which will set the GitHub topic in iCloud.
   - ![image 6](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/6.jpg)

4. **Add Scriptable Widget**:
   - Go to your iOS home screen.
   - Enter jiggle mode by holding an app icon.
   - Tap the "+" button in the top left corner.
   - Search for "Scriptable" and select it.
   - Choose a widget size (large) and add it to your home screen.

5. **Widget Configuration**:
   - Configure the Scriptable widget to run the `Scriptable-GithubRepo.js` script.
   - add this script (`Scriptable-GithubRepo.js) to your scriptable widget.
   - ![image 4](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/4.jpg)
   - after you have typed in the topic in your shortcut, Click on the scriptable widget icon to run the script.
   - The widget will automatically update with the top GitHub repositories for the specified topic.
   - ![image 8](https://github.com/Agrim-Ani/GithubTopRepos/blob/main/images/8.PNG)

## Project Structure

- **Shortcut-Script.js**: This Scriptable script is designed to be run by an iOS Shortcut. It saves the user's GitHub topic parameter to iCloud.

- **Scriptable-GithubRepo.js**: This Scriptable script creates the widget and fetches the top GitHub repositories based on the user's specified topic. It also displays the data in the widget.

## Customize the Project

- You can customize the appearance of the widget, such as its colors and fonts, by modifying the `createWidget` function in `Scriptable-GithubRepo.js`.

- To change the GitHub API request, update the `getTopRepositoriesByTopic` function in `Scriptable-GithubRepo.js`.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the Scriptable community for inspiration and support.
- GitHub API documentation for providing the data source for this project.

Feel free to contribute to this project or use it as a template for your own Scriptable widgets!

