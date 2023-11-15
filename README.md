![](https://github.com/swinnoproject/website/actions/workflows/publish.yml/badge.svg)

# Repo for SWINNO's website

## Usage

The easiest way to update this website is to edit a document directly on github.
[Log in](https://github.com/login) to github and o to the file that you wish to 
change make your changes and then click on the pen icon and begin editing.
When you are happy with the edit, click on the green button "Commit changes".
You will be prompted to write a commit message, but for simple changes you can accept the default that is already filled in.
Make sure that you commit directly in the main branch (the default option) and click on commit changes once more.
**That is it!**

A workflow should now be triggered that updates the websites.

It can take a few minutes for your changes to appear and do not forget to refresh your browser.
If it takes more than a few minutes for the change to occur, try loading the page in another browser before 
[reporting the issue](https://github.com/swinnoproject/website/issues/new).

### Example: Mangaging Team Member Pages

To illustrate how to add and change content, this section walks you step by step through creating a new file, changing existing files and uploading new files from your computer.

To ensure that we always have a working website, we use branches.
Branches are a useful feature in git and you can read more about them in many online tutorials like this [one](https://www.atlassian.com/git/tutorials/using-branches).
In short, you can think of branches like alternative universes of the entire project.
From the moment you create a branch, you create a new universe where all changes that you make only happen in that universe.
When you are happy with the changes we can introduce them into the main branch -- the one true universe so to say.
Below will introduce you two ways of creating and working with branches.

1. Creating a new file:

    Go to the folder in which you want to create a new file.
    To create a new current team member profile, go to  `team/current`.
    In the top right of the page you see a button `Add file`.
    Click on it and select `Create new file`.
    You can enter some content (see next step), cancel the file creation or "save" the new file by clicking on the green button `Commit changes`.
    Before you commit your changes, make sure that you are on the right branch.
    Do not commit directly to the main branch!
    Instead, at this point you can create a new branch by choosing the second option and giving it a name like "new-profile" or "change-profile-xyz".
    A new window opens where you can describe what you have changed, or simply commit by clicking on the green button again.
    Your changes will be sent to review, this way we can make sure that everything works as expected before publishing it to the website.

    ![](assets/images/create_file.gif)

2. Make changes to a file:

    Go to the file you want to change.
    Check if you are on the correct branch, or create a new branch by clicking on the button in the top left.
    If you have created a file on a new branch as described in step 1., you will not be able to see this file unless you are on the right branch.
    Once you are on the correct branch, click on the pen icon in the top right corner to begin editing.
    Make your changes.
    When you are done making your changes, click on the green `Commit changes` button, add or accept the message to go with the new changes.
    Make sure that you are adding the changes to the correct branch and click on commit again.

    ![](assets/images/update_file.gif)


    To help you get started creating a new personal profile, you can copy paste the template below and modify it.
    You can delete the links that you do not need (the two lines starting with - icon: / -text: and href:). 

        ---
        title: "First Last"
        subtitle: Role
        image: ../../assets/images/FirstLast.jpg
        about:
            template: broadside
            links:
                - icon: person-fill
                    href: link to personal website
                - icon: mortarboard-fill
                    href: link to google scholar
                 - text: "{{< ai orcid >}}"
                    href: link to your orcid profile
                - icon: twitter
                    href: link to social media
                - icon: mastodon
                  href: link to your mastodon
                - icon: github
                    href: https://github.com/first_last
                - text: "{{< bi envelope-fill >}}"
                    href: mailto:first_last@ekh.lu.se

        toc: false
        ---

        :::{.text-bigger}
        A short description.
        :::

3. Upload files from your computer

    Now, let's add an image.
    Pay attention that the image file name on your computer matches the name in `image: ../../assets/images/FirstLast.jpg`.
    In this case that would be `FirstLast.jpg`.
    Go to `assets/images` and click on `Add file` in the top right corner.
    This time, choose `Upload files`.
    Drag and drop, or search, for the file you want to upload.
    Click on commit as in the previous steps.

    ![](assets/images/upload_file.gif)
