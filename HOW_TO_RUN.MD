# Requirements

- [Python Anywhere Account](https://www.pythonanywhere.com/registration/register/beginner/)

[ That's it for free hosting ]

# Steps

- Create an account in Python Anywhere


![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fn6npxfuo38zhzalqc7b.png)


- Click on Web TAB and click on Add a new web app button in the left side

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8buxjadz9desioaws9z5.png)

- Click on Next button below

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tl4d7x9xakl070sdp9y9.png)

- Select flask from the options below

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4572p5yffv0fy5l1zjum.png)

- Select the latest python version from list

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1ydp8uan9pe531rfwsmd.png)

- Edit the file name of your project in the end. I'm editing with mine as **app.py**

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t8n2riwf3c8smmd0ejih.png)

- A new folder with /mysite will be created in our file manager. Click on Files TAB from the navigation bar. Click on the /mysite directory in the left corner.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/90aaney5a64m1231aej6.png)

- If you need to create directory, follow the left corner textbox, write the directory name & click New Directory button.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/uzqxfha9bqs72lrv4tws.png)


- Upload the files here.

N.B. - You can't upload multiple files at a time. Also, if there exist any directory, you need to create one & then upload files.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/irs11fdsi2q4evm8xaoh.png)

- Once again navigate to Web TAB & click on Reload USERNAME.pythonanywhere.com ; where USERNAME is your username

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/kds6gtm08lq65sa258e6.png)

- That's it. Your site is live now. Let's check mine!

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zo4bf0fqzvpgz7xqwsn2.png)

---
**Getting some error? Try some of the below debugging :**

- Try to update & install the libraries/modules which may not be installed in your Python Anywhere account.  
Navigate to the Files TAB & then to the /mysite folder & click on Open bash console here hyperlink.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3uydmf1xrh6j04vyw4ud.png)

2. Type the following command in console
`pip install -r requirements.txt`
[ If you have a requirements.txt file]

In case you don't have, check how to create one from [here](https://intellij-support.jetbrains.com/hc/en-us/community/posts/206603015-Can-pycharm-create-the-requirements-txt-file-what-am-I-missing-)

3. All the required dependencies will be installed.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/0kve0w1u38b4s0jqbcs6.png)

4. Now go back to Web TAB & click on Reload USERNAME.pythonanywhere.com ; where USERNAME is your username.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rhwkbeyl2f50v31wrrdo.png)

- Another is the config file. We call it as WSGI config file. You could find it in Web TAB only.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/wwnzkyxxuumsg2f2qh8o.png)

1. Click on the file name to edit the config file.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w8hmjygs3ynqyzsf3fqr.png)

2. Check all the contents should be like below code:

```
import sys

# add your project directory to the sys.path
project_home = '/home/name01001/mysite'
if project_home not in sys.path:
    sys.path = [project_home] + sys.path

# import flask app but need to call it "application" for WSGI to work
from app import app as application  # noqa
```

3. Click on Save button

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/r1zcmbkqerwi1e0hbolg.png)

4. Now go back to Web TAB & click on Reload USERNAME.pythonanywhere.com ; where USERNAME is your username.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rhwkbeyl2f50v31wrrdo.png)


I've tried to teach how to host Python (Flask) app for free in the simplest manner possible. However, if you're facing any difficulty, do mention it in the comment. Wil try to help. 

You can follow me on [LinkedIn](https://linkedin.com/in/nitin30kumar/), [Instagram](https://instagram.com/nitinkuamr30.py/) or check my latest projects on my [GitHub](https://github.com/nitinkumar30/). Also, you can check my [portfolio](https://nitin-kr.onrender.com/) too. 

[Keep Coding] [Thanks]





















