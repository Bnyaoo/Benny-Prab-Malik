---
layout: default
title: Writing a Basic Function
nav_order: 2
has_children: false
permalink: /docs/navigating
---

{: .fs-6 .fw-300 }

# Writing a Basic Function
{: .no_toc }

---

Python is capable of programming many tasks, but before we can create our own projects we need to learn the basics. This section of the guide will walk you through how to create a basic palindrome function and run the file in the command line. We want to help you develop good programming habits, so we will guide you through how to write comments, docstrings and doctests to ensure your code is able to detect a palindrome word.

---

### Table of contents
{: .no_toc .text-delta }
* TOC
{:toc}

---

## Things You Should Pay Attention To:

* Ensure that each block statement is indented (ex. Everything inside function is indented once, everything inside an if statement is indented 1 level further)
* Each opening paranthesis has a closing paranthesis
* Each conditional statement and function header is followed with a colon
* Everything is typed correctly, without typos

---

## Command Table

Below is a list of some commands that will be needed to follow along with this document.

**Note**: We will be using the terminal built into the PyCharm IDE.

| Command         | Description                                                                                             |
| :--------       | :------------------------------------------------------------------------------------------------------ |
| `#`             | Any text after an octothorpe (pound symbol) will be a comment, therefore it will not be executed        |
| `clear`         | "Clear" your terminal screen.                                                                           |
| **[Enter]**     | Processes the command that has been typed                                                               |

---

## Writing a Palindrome Function

One of the most common introduction problems that developers solve is determining if a string is a palindrome or not. A palindrome is a word, phrase, or sequence that reads the same backward as forward.

---

**1.** Open the Pycharm application by clicking the icon from the launchpad.

>![img1](https://user-images.githubusercontent.com/90500768/161899986-b0b0c2b5-2736-41b2-9986-287a625c7551.png?raw=true "PyCharm")
<br />
<br />

**2.** Click “New Project” in the top right corner of the screen.

>![img2](https://user-images.githubusercontent.com/90500768/161901139-48deb548-5d2e-462d-a249-3b3003eee5a2.png?raw=true "Creating New Project")
<br />
<br />

**3.** Delete the highlighted section with “palinedromeProject” and confirm that the “create a main.py welcome script” is selected.

>![img3_pt1](https://user-images.githubusercontent.com/90500768/161901437-1346111d-1d50-4d18-a2f1-8293cb180ddd.png?raw=true "Set uUp New Project")
<br />
>![img3_pt2](https://user-images.githubusercontent.com/90500768/161901519-7a1887dc-b8b1-4d93-9f34-4bf6ad4b5eae.png?raw=true "Set Up New Project")
<br />
<br />

**4.** Click “create” on the bottom right corner.

>![img4](https://user-images.githubusercontent.com/90500768/161901721-ddbae822-d61c-4c63-a136-70f91b710d20.png?raw=true "Create New Project")

**5.** Highlight and delete the existing code to start coding from scratch.

>![img5_pt1](https://user-images.githubusercontent.com/90500768/161901865-3b5a37a9-3e38-4306-804c-221c7b697bb2.png?raw=true "Delete Existing Code")

<br />
>After you delete all the existing code you should have a blank file like the image below.
<br />

>![img5_pt2](https://user-images.githubusercontent.com/90500768/161902193-181f557f-6e35-40dd-be20-3b4ff7dcf792.png?raw=true "Empty File")

<br />
<br />

**6.** Type the following code.

>![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
>> **Note**: Ensure that each block statement is indented (ex. Everything inside function is indented once, everything inside an if statement is indented 1 level further)
<br />
<br />

~~~
import sys  # allows us to use command line arguments


def palindrome(word):
    # checks to see if the provided string is an empty string
    if len(word) == 0:
        print("Please enter a non-empty string")
        exit(0)

    # Checks if the provided string is just one letter
    if len(word) == 1:
        return True

    # checks the first and last index of the word (converts both letters to lowercase to avoid error)
    if word[0].lower() == word[-1].lower():
        # Recursively calls the function to make sure the first half of the string mirrors the second half of the string
        return palindrome(word[1: -1])
    # if the word is not a palindrome return false
    else:
        return False


def main():
    # takes the command line argument and stores it in the variable word
    word = sys.argv[1]
    # calls the function we created and stores the return time in a variable called isPalindrome
    isPalindrome = palindrome(word)
    # prints out the return value
    print(isPalindrome)


# Allows us to run the file only if it has been executed not imported
if __name__ == "__main__":
    main()

~~~

>The file should now look like the image below.
<br />

>![img7](https://user-images.githubusercontent.com/90500768/161904702-c28a9bf6-6f68-476e-becc-9f5d6964727e.png?raw=true "Completed Code")

<br />
<br />

**8.** Press the terminal button at the bottom of the screen.
<br />
<br />
>![img8](https://user-images.githubusercontent.com/90500768/161905803-f880011b-0aab-439c-aac1-9284e71c95b8.png?raw=true "Open Terminal")

<br />
<br />

**9.** Type the following command.
<br />
>![Note icon](https://github.com/dl90/linux-basics/blob/gh-pages/docs/images/icons/note.png?raw=true "Note"){: style="float: left" }
>> **Note**: The string `bob` below can be replaced with any string of your choice.
<br />
<br />
>```
>python main.py bob
>```

<br />
>![img9](https://user-images.githubusercontent.com/90500768/161905959-bffa6619-36f1-4b1a-baab-d99158542d56.png?raw=true "Type Command")

<br />
<br />

**10.** Press the [enter] key to run the command
>The command in step 9 should return true like the image below.
<br />
<br />
>![img10](https://user-images.githubusercontent.com/90500768/161906102-82d40917-c91a-414d-a070-4cdcf2a70ab9.png?raw=true "Enter Command")

<br />
<br />

Now that the code is complete you can repeat steps 9 and 10, but with a new string to execute your program.

The next step is to learn how to unit test your program.
