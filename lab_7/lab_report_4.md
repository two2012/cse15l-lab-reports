# Lab Report 4

### 1. Setup Delete any existing forks of the repository you have on your account 

* `rm -rf lab7 # remove existing lab7 floder`
* `<enter>`
* `ls` 
* `<enter>`

    ![Alt text](img/remove%20lab7.png)

### 2. Setup Fork the repository

   ![Alt text](img/fork1.png)

   ![Alt text](img/fork2.png)


### 3. The real deal Start the timer!


### 4. Log into ieng6

* `ssh cs15lwi23alv@ieng6.ucsd.edu`
	* Note: I skip the time to type the password when I login to ieng6, because I generate a SSH keys for ieng6.
* `<enter>`

    ![Alt text](img/login.png)

### 5. Clone your fork of the repository from your Github account

* `git clone git@github.com:two2012/lab7.git`
* `<enter>`
* `ls`
* `<enter>`
* `cd l<tab>`
	* Note: this command is to change the directory to lab7 

    ![Alt text](img/clone.png)


### 6. Run the tests, demonstrating that they fail

* `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`
* `<enter>`
* `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore L<tab>T<tab>`
* `<enter>`

    ![Alt text](img/test%20fail.png)


### 7. Edit the code file to fix the failing test

* `nano L<tab>.j<tab>`
	* Note: the first <tab> will stop at ListExamples. because there are two files match this partten, the one is ListExample.java the other one is ListExample.class. so I type j<tab>
* `<enter>`

    ![Alt text](img/nano1.png)

* `<ctrl> + <w>`
	* Note: this keystroke is to search for keyword, in this way I can find what I want very quick.
* `result.add`
* `<enter>`
* `<right> x 13`
* `<back> x 3`
* `<ctrl> + <w>`
* `index1 += 1;`
* `<enter>`
* `<right> x 6`
* `<back>`
* `2`
* `<ctrl> + <o>`
	* Note: this keystroke is to save what I change to the file.
* `<enter>`
* `<ctrl> + <x>`
	* Note: this keystroke is to exit out to nano file editing.


### 8. Run the tests, demonstrating that they now succeed

* `<up> x 3`
* `<enter>`
* `<up> x 3`
* `<enter>`

    ![Alt text](img/test%20pass.png)


### 9. Commit and push the resulting change to your Github account

* `git add L<tab>.j<tab>`
* `<enter>`
* `git commit -m "fixed"`
* `<enter>`

    ![Alt text](img/add%20and%20commit.png)

* `git push`
* `<enter>`

    ![Alt text](img/push.png)




