---
layout: default
title: Writing a unittest
nav_order: 3
has_children: false
permalink: /docs/customization
---

{: .fs-6 .fw-300 }

# Writing a Unit Test 
{: .no_toc }

---

After learning the basics of writing a function and running the file from the command line, we want to test the function to help you find and fix any bugs that may be in the code. We will be unit testing the palindrome program that you wrote on the previous page to make sure that the program is working as intended. Unit testing is very important because it helps developers write better code more efficiently. 

---

### Table of contents
{: .no_toc .text-delta }
* TOC
{:toc}

---

## Writing a Unit Test for a Palindrome Function

Unit testing is a technique in which particular module is tested to check by developer himself whether there are any errors. The primary focus of unit testing is test an individual unit of system to analyze, detect, and fix the errors. In this section you will be creating a unit test for the palindrome created in the previous section.

---

**1.** On your main python file that contains the palindrome function, right-click on your mouse and click “Generate”.

![1](https://user-images.githubusercontent.com/18428358/161939376-e2bb3191-e70e-4395-b59a-6fb71230c662.png?raw=true)

<br />
<br />

**2.** Click on “Tests…” and Pycharm will show you the available methods that can be tested.

![2](https://user-images.githubusercontent.com/18428358/161939618-60558062-ed5c-42e4-bc25-c2a5085ca7c1.png?raw=true)

<br />
<br />

**3.** Name the Test file and Test class as shown below, don’t forget to select the function that we will be testing by clicking the checkbox next to your desired test function. 

![3](https://user-images.githubusercontent.com/18428358/161940229-4772a175-9f35-4671-8e0d-8c7040e0f745.png?raw=true)

<br />
<br />

**4.** Click “OK” when you are ready to proceed. 

![4](https://user-images.githubusercontent.com/18428358/161940647-46c14c4e-cb9c-45cd-a8d9-dc89994568e5.png?raw=true)

<br />
<br />

**5.** After clicking “OK”, Pycharm will create a new .py file where we can test our palindrome function. 

![5](https://user-images.githubusercontent.com/18428358/161940828-542749aa-6e72-4895-af7f-eca1702ecec3.png?raw=true)

<br />
<br />

**6.** Add this line of code on line number 2 which will be grayed out upon writing it down, for now.

~~~
from main import palindrome as palindrome

~~~

This line of code is calling the palindrome function from main.py.

![6](https://user-images.githubusercontent.com/18428358/161941225-33a89221-8e25-44c2-b682-d19fa1d242db.png?raw=true)

<br />
<br />

**7.** Delete lines 6 and 7 as we will be making our own unit tests. 

![7](https://user-images.githubusercontent.com/18428358/161941664-56db6352-e051-47d6-94e4-f01fb7978a65.png?raw=true)

<br />
<br />

**8.** Type the following blocks of code starting at line 6.

~~~
    def test_palindrome_with_all_lower_case(self):
        expected = True
        actual = palindrome("civic")
        self.assertEqual(expected, actual)

    def test_palindrome_with_same_letters_but_different_cases(self):
        expected = True
        actual = palindrome("Civic")
        self.assertEqual(expected, actual)

    def test_palindrome_with_input_that_is_not_a_palindrome(self):
        expected = False
        actual = palindrome("abc")
        self.assertEqual(expected, actual)
        
~~~
        
After adding these lines of code, the whole testing file should look like the image provided below.

![8](https://user-images.githubusercontent.com/18428358/161942196-25f598df-5d08-4647-a8cf-c55841ba64c8.png?raw=true)

<br />
<br />

**9.** To check if the function are working properly, right click next to your code and select, “Run ‘Python tests for tes…’ ”. 

![9](https://user-images.githubusercontent.com/18428358/161943842-93177f0f-9f43-415f-b7dd-df57fa24bcef.png?raw=true)

<br />
<br />

**10.** If done correctly all 3 tests should pass and green checkmarks will appear at the bottom of PyCharm to indicate our function is working properly. 

![10](https://user-images.githubusercontent.com/18428358/161944517-395a072f-63cc-447a-8148-aa4aa28f2e63.png?raw=true)

<br />
<br />

Congratulations you have passed all the tests. There are more ways you can test out your functions which you can explore yourself. 

Now the next step is creating and pushing a project to a Github Repository.
