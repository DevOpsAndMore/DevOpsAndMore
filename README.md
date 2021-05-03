Books for beginners:
<description>
  
1. A bity of Python

Visit https://github.com/swaroopch/byte-of-python/releases/latest to download a PDF file (best for desktop reading) or an EPUB file (best for devices such as mobile, tablet, ebook readers).

Visit https://github.com/swaroopch/byte-of-python for the raw content (for suggesting corrections, changes, translating, etc.)

Read the book in your native language
If you are interested in reading or contributing translations of this book to other human languages, please see Translations.
</desciprion>

Most useful python modules for DevOps:
<details>

1. Requests

This module allows you to send HTTP requests. Using this module, we can post or retrieve the data from a Rest API. There are many methods included in this module, like:

GET
POST
PUT
DELETE
All these methods perform particular actions like adding a comment (PUT), retrieving data (GET), or deleting a user field (DELETE).

Example:  r = requests.get(“url”,auth=('username', 'passwd'))

In the above example, we used the request module to get the information from the URL provided. You can get information like status code, JSON data using status code() and json() methods, respectively.

2. Paramiko

The Paramiko module allows users to log in to a virtual machine’s server using automation scripts. It enables the users to perform ad-hoc commands by using SSH client. All commands get executed in the connected remote machines.

Example - ssh = paramiko.SSHClient()
          ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
          ssh.connect(ip, username=user, password=passwd)
          stdin, stdout, stderr = ssh.exec_command("command")
          out = stdout.readlines()

In this example, we connected to a server using its I.P., username, and password. ‘stdin’ stores the input passed, ‘stdout’ stores the output obtained, and ‘stderr’ stores the error occurred.

3. Pandas

Pandas module is for data manipulation. It is the most useful module for data science engineers. But in DevOps, Pandas helps to store the massive dump of data into CSV or Excel files within seconds.

Example - pandas.read_json("file.json").to_excel("output.xlsx")

In the above example, we used the read_json() method to read a JSON file and migrated its data into an Excel file.

4. Selenium

One of the most popular modules used in Python to perform testing and connect to different browsers. By using Selenium, we can hit a URL and perform actions like clicking on a button. We can even use other sub-modules like ‘Pyautogui’ with Selenium for different purposes, like filling some text fields.

Example - from selenium import webdriver
          driver = webdriver.Chrome()
          driver.get("https://www.gspann.com")

In the above example, we have used Chrome WebDriver to access the Chrome browser. If you want to use this module for other browsers, you need to use different WebDrivers accordingly.

5. BeautifulSoup

It is the most useful module in Python for pulling data from HTML and XML files. To parse data from the content in HTML and XML format, we need to create a BeautifulSoup object for it. We can then use the BeautifulSoup methods on the soup object that we created for the URL. We can even apply many filters using the tags on the obtained data content, like soup.find_all(“< tag>”).

Example - URL = “https://www.gspann.com”
          content = urllib2.urlopen(url).read()
          soup = BeautifulSoup(content)

In this example, we are extracting all the content of the page into a soup variable. Using the soup variable, we can obtain the information of a specific tag by methods like find_all.

6. OS

This is the basic module used in python. It performs ad-hoc commands on the base OS, which we are executing. All commands run on the current machine.

Example -  os.system(“dir”)

In the above example, ‘dir’ gives an output of the list of directories. They are many other similar methods like os.remove(), os.rename(), os.close(), etc.

7. JSON

JSON is the syntax for storing data in the form of dictionaries and lists. Python has a built-in module named JSON. Using this module, we can parse the JSON data and even convert the other type of data into JSON format.

Example - 
			x = {
			      [“data”,”stored”]
			    }
			json.dump(x)

In this example, we can observe that x is a dictionary that is holding a list containing elements. We are using the dump function to parse the data.

8. XLWT

This module helps to create an Excel file and store data after customizing it according to the cells. It is a good module to work with Excel files, but it takes more time when compared to the Pandas. This module allows the user to define the logic according to the requirement, like filling data only in a particular cell.

Example - 
			x=Workbook()
			sheet=x.add_sheet()
			sheet.write()

In the above example, we initialized an Excel workbook in a variable and started performing actions like adding a sheet and writing data into that sheet using that variable.

Python helps us in automating repetitive things and it offers a lot of flexibility. It has a small learning curve compared to other programming languages. However, it all depends on how much time and effort a DevOps engineer spends on aptly utilizing its different modules, methods, and frameworks to enable automation. It will be apt to say that Python is core to DevOps automation and mastering this language is necessary to enable DevOps.
</details>
