mc## Advanced Command Line and Shell Scripting

![simpsons grocery store](https://metrouk2.files.wordpress.com/2015/06/simpsons-2.gif)

You've just been hired by your local grocery store to stock all the shelves with a delivery that has come in from the warehouse. Congratulations on your new job.

### Get the files
There are a couple of ways you can get these files. Choose the method that works for you. You can click `Open` at the top of this page. You could also go to the GitHub link at the top of the lab and, if you are familiar with Github already, clone the repo locally. Otherwise, click on the "Clone or Download" button then the "Download Zip" button on the right side of the screen. Once you've downloaded the file, double click it to unzip the file, and then drag the unzipped file (called 'kwk-l1-advanced-cli') to your development directory.

## Part 1: Write a shell script
You've learned about the different commands in your terminal (`ls`, `mv`, `rm`, `mkdir`, `touch`, etc), but now we're going to learn how to string these commands together by using **bash scripting**. A _bash script is essentially a file with a set of instructions inside of it that when called from the command line will run the commands in the order in which they are written in the file_. For example, in your development directory create a file called `test_script.sh`. Open this file in the text editor and add the follwing to the contents of the file:

```bash
ls;
mkdir this_is_a_directory_made_in_a_script;
mkdir another_directory;
touch this_is_a_directory_made_in_a_script/first_file.txt;
touch this_is_a_directory_made_in_a_script/second_file.txt;
mv this_is_a_directory_made_in_a_script/second_file.txt another_directory

```

Save and close the file and then run it in your terminal by typing `sh test_script.sh`. This will run all the commands in this bash script. From the `kwk-l1-advanced-cli` directory, run `learn` as usual to check your progress!

### Challenge 1
Using the mini-lesson above, write a bash script that will put all of the files in the delivery directory in their right locations. As part of the challenge:
- You cannot `cd` into any directories, you must stay in the root directory of the project.
- All