# CRUD_Web_Application
Complete Crud Web application !

# Repository Title Goes Here

> This is CRUD (Create, Read, Update, Delete) application website

> #php


***INSERT ANOTHER GRAPHIC HERE***

[![INSERT YOUR GRAPHIC HERE](http://i.imgur.com/dt8AUb6.png)]()

- Most people will glance at your `README`, *maybe* star it, and leave
- Ergo, people should understand instantly what your project is about based on your repo

> GIF Tools

- Use <a href="http://recordit.co/" target="_blank">**Recordit**</a> to create quicks screencasts of your desktop and export them as `GIF`s.
- For terminal sessions, there's <a href="https://github.com/chjj/ttystudio" target="_blank">**ttystudio**</a> which also supports exporting `GIF`s.

**Recordit**

![Recordit GIF](http://g.recordit.co/iLN6A0vSD8.gif)

---

## Table of Contents (Optional)

> If your `README` has a lot of info, section headers might be nice.

- [Installation](#installation)
- [Features](#features)
- [Contributing](#contributing)
- [Team](#team)
- [FAQ](#faq)
- [Support](#support)
- [License](#license)


---

## Installation

First you need to have a local server environment like MAMP or XAMP.<br /><br />
1] Download the whole github folder in your htdocs folder<br />
2] Go on your PHPmyAdmins page and create a new database named crud<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (you can use the following code : CREATE DATABASE crud DEFAULT CHARACTER SET utf8 ;)<br />
3] Go in Sql interface of this DataBase and copy paste the following Sql querrys :<br />
  
  GRANT ALL ON crud.* TO 'Admin'@'localhost' IDENTIFIED BY '1234';<br />
  GRANT ALL ON crud.* TO 'Admin'@'127.0.0.1' IDENTIFIED BY '1234';<br />

  CREATE TABLE users (<br />
    user_id INTEGER NOT NULL AUTO_INCREMENT,<br />
    name VARCHAR(128),<br />
    email VARCHAR(128),<br />
    password VARCHAR(128),<br />
    PRIMARY KEY(user_id),<br />
    INDEX(email)<br />
  ) ENGINE=InnoDB CHARSET=utf8;<br />

  ALTER TABLE users ADD INDEX(email);<br />
  ALTER TABLE users ADD INDEX(password);
<br />
  INSERT INTO users (name,email,password) <br />
  VALUES ('UserDefault','vincent.bernet@efrei.net','1a52e17fa899cf40fb04cfc42e6352f1');<br />

  INSERT INTO users (name,email,password) 
  VALUES ('UMSI','umsi@umich.edu','1a52e17fa899cf40fb04cfc42e6352f1');

TODO: End of SQL Querrys

4] Go to pdo.php file and change the port number to 8808 <br/>
(only if you are on Mac or if your local server environment default port number is not 3306)  :
&nbsp;&nbsp;&nbsp; ![Pdo.php](Screenshot_ReadMe/Pdo.JPG)

5] Run the index.php file on your browser, if no SQL error's statement pop everything work !
If there is some error check your database and your port number.

## Features
## Usage (Optional)
## Documentation (Optional)
## Tests (Optional)

- Going into more detail on code and technologies used
- I utilized this nifty <a href="https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet" target="_blank">Markdown Cheatsheet</a> for this sample `README`.

---

## Contributing

> To get started...

### Step 1

- **Option 1**
    - 🍴 Fork this repo!

- **Option 2**
    - 👯 Clone this repo to your local machine using `https://github.com/joanaz/HireDot2.git`

### Step 2

- **HACK AWAY!** 🔨🔨🔨

### Step 3

- 🔃 Create a new pull request using <a href="https://github.com/joanaz/HireDot2/compare/" target="_blank">`https://github.com/joanaz/HireDot2/compare/`</a>.

---

## Team

> Or Contributors/People

| <a href="http://fvcproductions.com" target="_blank">**FVCproductions**</a> | <a href="http://fvcproductions.com" target="_blank">**FVCproductions**</a> | <a href="http://fvcproductions.com" target="_blank">**FVCproductions**</a> |
| :---: |:---:| :---:|
| [![FVCproductions](https://avatars1.githubusercontent.com/u/4284691?v=3&s=200)](http://fvcproductions.com)    | [![FVCproductions](https://avatars1.githubusercontent.com/u/4284691?v=3&s=200)](http://fvcproductions.com) | [![FVCproductions](https://avatars1.githubusercontent.com/u/4284691?v=3&s=200)](http://fvcproductions.com)  |
| <a href="http://github.com/fvcproductions" target="_blank">`github.com/fvcproductions`</a> | <a href="http://github.com/fvcproductions" target="_blank">`github.com/fvcproductions`</a> | <a href="http://github.com/fvcproductions" target="_blank">`github.com/fvcproductions`</a> |

- You can just grab their GitHub profile image URL
- You should probably resize their picture using `?s=200` at the end of the image URL.

---

## FAQ

- **How do I do *specifically* so and so?**
    - No problem! Just do this.

---

## Support

Reach out to me at one of the following places!

- Website at <a href="http://fvcproductions.com" target="_blank">`fvcproductions.com`</a>
- Twitter at <a href="http://twitter.com/fvcproductions" target="_blank">`@fvcproductions`</a>
- Insert more social links here.

---

## Donations (Optional)

- You could include a <a href="https://cdn.rawgit.com/gratipay/gratipay-badge/2.3.0/dist/gratipay.png" target="_blank">Gratipay</a> link as well.

[![Support via Gratipay](https://cdn.rawgit.com/gratipay/gratipay-badge/2.3.0/dist/gratipay.png)](https://gratipay.com/fvcproductions/)


---

## License

[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](http://opensource.org/licenses/mit-license.php)**
- Copyright 2015 © <a href="http://fvcproductions.com" target="_blank">FVCproductions</a>.