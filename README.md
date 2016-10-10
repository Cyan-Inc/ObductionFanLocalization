# ObductionFanLocalization
Localized changes to the game Obduction.

Hello there!
Thank you so much for your interest in contributing localization support for a new language in Obduction!
Feel free to fork our repository and make a pull request in adherance to the [standards listed in our FAQ](https://github.com/Cyan-Inc/ObductionFanLocalization/wiki/FAQ#what-information-or-data-do-i-need-to-include-in-my-pull-request), and some are listed here for reference:
### I want to localize files from Obduction into a new language. How do I go about doing this?
1. In your game's `Obduction/Content/Localization` directory, add a new directory for your language named as two letters that are generally used as describing your language name (e.g. "fr" would be two characters that in general use, symbolize "French").
2. Copy and paste all of the files from the `en` directory into your new language.
3. Add a new language entry in your `Languages.json` file (in the `Localization` directory) with a `LanguageID` that is the same as the name of the directory you just created (that is how the localization manager in the game finds your files), a `LanguageName` that is the English translation of your language name, and a `DisplayName` that is the name of your language in your language.
4. Open Obduction and verify that your language appears in the languages list in the menu. If it is not listed in the languages list, double check that you entered everything in the `Languages.json` file correctly.
5. Start translating files in your new language's directory and be sure to check that they work in-game. Please note that all files must be saved with an encoding of UTF-16 LE with BOM. (Note: We know that `git diff` currently treats these files as binary files, and we are looking into alternative, reliable solutions on our end to get around this issue and make it easier for people to contribute, but for now, UTF-16 files will be what we accept).
6. Once all of your files are translated and have been verified as displaying correctly in the game, you can make a pull request into this repository with that folder you created.

### I'm unfamiliar with GitHub, but I would like to contribute a language I've localized for Obduction by making this so-called "Pull request". How can I share my work with you?
1. Create a GitHub account.
2. Visit [our repository's Localization directory](https://github.com/Cyan-Inc/ObductionFanLocalization/tree/master/Localization).
3. Click on the "Upload Files" button that is sitting just above the "latest commit" message, near the top right of the screen.
4. Drag the folder on your disk that contains your new language's localized files into the area that says "Drag files here".
5. Once you have done that, scroll down and enter in a title and commit message for your commit.
6. When you have added your title and commit message in accordance to our README, click on "Create Pull Request".
7. On the page you are brought to when creating a pull request, ensure that the base fork (the fork on the left) is the `Obduction Fan Localization` repo and the branch next to it is `master`.
8. Ensure that your title and commit message are good enough to submit, and then press "Create a Pull Request" again.
9. For more information on using GitHub and creating pull requests, see [GitHub's start-up guide.](https://guides.github.com/activities/hello-world/).

### What information or data do I need to include in my pull request?
*Information* included in your commit message:
* Your **email address** that we may use to contact you directly
* Your **name or identifier** (can be a username you go by), and -- if applicable -- the name or identifier of person(s) whom you are contributing on behalf of (and please include a link to their specific written permission for you to do so)
* The **language ID** (two character identifier) of the language you are adding localization support for (like in the `Languages.json` file)
* The **display name** (and dialect, if applicable) of the language you are adding localization support for (like in the `Languages.json` file)
* The **language name** (and dialect, if applicable) of the language you are adding localization support for (like in the `Languages.json` file)
* Which **version of Obduction** you used to test your translations
* A **short summary** (1-2 sentences) about your translation approach

*Data* included in your pull request:
* **New language's localization folder that has all files translated to the language desired**
* Optional: If desired, a .txt file of a longer summary of your localization approach and notes (placed within your language's new directory)

### Do I need to test my new language support in my local copy of the game before making a pull request?
Yes.

