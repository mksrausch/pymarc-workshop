## Instructions:

Prerequisite: You have installed Python onto your computer with pip and PyMarc.
* Mac OSX Instructions:  http://docs.python-guide.org/en/latest/starting/install3/osx/
* PC Instructions: http://docs.python-guide.org/en/latest/starting/install3/win/
* PyMARC installation instructions: https://github.com/edsu/pymarc
  * Note: if you see the error "command not found" using pip, try `python -m pip install pymarc` (thanks to Rachel Tillay @ Tulane for this tip!)


1. Download this GitHub repository onto a place you can easily access (e.g., Documents) on your command line tool (Terminal (OSX) or PowerShell (PC)).  
2. Unzip it.
3. Open your command line interface (Terminal on Mac, PowerShell on PC) and navigate to the place you downloaded the directory.  If in the Documents directory:
* On a PC, try `cd C:/Users/yourusername/Documents/pymarc-workshop-master` (cd stands for "change directory"; make sure to swap out yourusername for your actual username, e.g., jsmith) 
* On a Mac, try: `cd /Users/yourusername/Documents/pymarc-workshop-master`
* Other useful commands to know:
  * pwd (outputs your current location on your computer/server)
  *  ls (lists the contents of a directory)
* To run the first python script, type into the command line:
* `python oclc1.py` (or `python3 oclc1.py`)

You should see the following output:

```
ocn318875078-01cals_network
ocn668941926-01cals_network
ocm59231572-01cals_network
ocn174040370-01cals_network
ocm52381684-01cals_network
ocn701325822-01cals_network
```

4. To run the second script, type into the command line:

`python3 oclc2.py`

You should see the following output:

```
318875078
668941926
ocm59231572
174040370
ocm52381684
701325822
```


### Activity 1:
How can you adjust the oclc2 script to get rid of the ocm prefix in two of the items?


### Activity 2:
Regular expressions can be used to evaluate a text string (like an OCLC number), 
look for a pattern, and modify the text string based on that pattern.

For example, a regular expression that would only match numbers looks like this:

[^0-9]

Python has a regular expression library called ‘re’ that you can include in your script in order to use Regular Expressions.  Take a look at the file  oclc-regex.py and run it in your command line.  What does this use of re do to the OCLC numbers in in the file?

### Activity 3:
Like re, csv is a Python library.  It makes it easy to output data to a CSV (comma-separated values) file.

Run the oclc-regex-csv script and see what happens (hint: look in the directory where you’ve downloaded this code for a file that wasn’t there before).

Can you modify the script (oclc-regex-csv) to output author information from the 245 |c as well as title information?

### Activity 4:
Examine and run isbn-gobi.py.  In the comments in the code, there are two loops (loop 1 and loop 2).  What does each loop do?







