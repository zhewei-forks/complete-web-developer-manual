# Complete-Web-Developer-Manual

All resources and notes from the Complete Web Developer in 2020: Zero to Mastery course

******************************************************************************************
## 1.	__Introduction__

Discord Channel:
*	https://discord.gg/nVmbHYY
******************************************************************************************
## 2.	__How The Internet Works__

Tools:
*	Chrome Developer Tools

Topics:
*	ISP, DNS and Servers
*	Traceroute (Windows: tracert)

Submarine Cable Map:
*	https://www.submarinecablemap.com/
******************************************************************************************
## 3.	__History Of The Web__

Maps that explain the Internet:
*	https://www.vox.com/a/internet-maps

First Webpage in the world:
*	http://info.cern.ch/hypertext/WWW/TheProject.html

Optional Videos:
*	https://www.youtube.com/watch?v=3QhU9jd03a0&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo&index=29
*	https://www.youtube.com/watch?v=AEaKrq3SpW8&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo&index=30
*	https://www.youtube.com/watch?v=guvsH5OFizE&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo&index=31

******************************************************************************************
## 4. __HTML 5__

Tags:
```
<!DOCTYPE html>
<html>
    <head> 
       <title> Title </title>
    </head>
    <body>
        Main contents
    </body>
</html>
```

*	headings (`h1`, `h2`, `h3`, `h4`, `h5`, `h6`)
*	paragraph `<p>`
*	bold `<strong>`, italic `<em>`
*	ordered list `<ol>`, unordered list `<ul>`, list item`<li>`
*	break `<br>`, horizontal line `<hr>`
*	image `<img src="~" alt="~" width="42" height="42">` 
*	anchor `<a href="www.google.com"> Link Name </a>`

******************************************************************************************
## 5.	__Advanced HTML 5__
```
<form method="POST" action="action.php">
    Name: <input type="text" name="name"><br>
    Email: <input type="email" name="email" required><br>
    Password: <input type="password" name="password" minlength="5" required><br>
    Birthday: <input type="date" name="birthday"><br>
    
    Gender:<br>
    <input type="radio" name="gender" value="Male">Male<br>
    <input type="radio" name="gender" value="Female">Female<br>
    <input type="radio" name="gender" value="Others">Others<br>
    
    Pets:<br>
    <input type="checkbox" name="cat">cat<br>
    <input type="checkbox" name="dog">dog<br>
    
    Cars:<br>
    <select name="cars">
    	<option value="volvo">Volvo</option>
	<option value="audi">Audi</option>
    </select><br>
    
    <input type="submit" value="Register">
    <input type="reset">
</form>
```

Tags:
*	`<form>`
	*	`method`, `action`
*	`<input>`:
	*	`type`= `"text"`, `"submit"`, `"reset"`, `"email"`, `"date"`, `"radio"`, `"password"`
	*	`required`, `value`, `name`, `min`
*	dropdown `<select>`
	*	option `<option>`
*	comment `<!-- -->`
*	paragraph/inline selection `<div>`, `<span>`

Semantic Elements
*	`<header>`
*	`<nav>`
*	`<main>`
*	`<footer>`

Topics:
*	Chrome view Source

Resources:
*	https://learn.freecodecamp.org/responsive-web-design/basic-html-and-html5
*	https://waitbutwhy.com/

******************************************************************************************
## 6.	__CSS__

Syntax:
```css
Selector {
	property: value;
}
```

How to:
*	External
	```html
	<link rel="stylesheet type="text/css" href="style.css">
	```
*	Internal
	```html
	<style>
		body {
			background-color: purple;
		}
	</style>
	```
*	Inline
	```html
	<header style="background-color: green;">
	```

Tools:
*	Chrome Inspector

Properties:
*	text-align
*	border
*	background
*	list-style
*	cursor
*	color: html, hex, rgb or rgba

Selectors: Cascading Style Sheets at the most basic level it indicates that the order of CSS rules matter.

| Selector      | Example       | Examples  |
| :-------------: |-------------| ---------|
| .class      | `.intro`   | Selects all elements with class="intro"   |
| .class1.class2      | `<div class="name1 name2">...</div>` | Selects all elements with both name1 and name2 set within its class attribute     |
| .class1 .class2 | `<div class="name1"> <div class="name2"> ...</div> </div>` | Selects all elements with name2 that is a descendant of an element with name1     |
| #id | `#firstname` | Selects the element with id="firstname"     |
| *   | * | Selects all elements     |
| element      | `p` | Selects all `<p>` elements |
| element,element | `div, p` | Selects all `<div>` elements and all `<p>` elements     |
| element element    | `div p` | Selects all `<p>` elements inside `<div>` elements     |
| element>element    | `div > p` | Selects all `<p>` elements where the parent is a `<div>` element     |
| element+element    | `div + p` | Selects all `<p>` elements that are placed immediately after `<div>` elements     |
| element1~element2  | `p ~ ul` | Selects every `<ul>` element that are preceded by a `<p>` element     |


Text Properties
*	`text-decoration` : i.e., `line-through`
*	`text-transform` : i.e., `uppercase`
*	`line-height` : i.e., `20px`
*	`font-style` : i.e., `italic`
*	`font-weight` : i.e., `bold`
*	`font-size`: i.e, `100%`, `150%`
*	`font-family` : i.e, `Georgia`, `"Times New Roman"` (can have multiple, refer to https://fonts.google.com/ and find some good fonts! Insert the link in the headeer)

Layout Properties
*	`float` : i.e., `left` with picture wrapped with texts and align to the left 
*	`clear` : i.e., `both` usually comes with float, , to clear the float setting 

Box Model
*	`content -> padding -> border -> margin`
*	`display` : i.e., `inline-block`
*	`padding` : i.e., `20px` or `5px 20px 5px 20px` for top, right, bottom and left
*	`margin` : i.e., `10px 5px` for top/bottom and left/right
*	`width` and `height`: change for contents
*	`border`

Sizes
*	`px`
*	`em` and `rem` : compare to the text size, for example: 5em means 5 times the fontsize (relative), rem compares to root element html

Topics:
*	Cascading: Specificity, Importance `!`, Source Order
*	Linking fonts and external stylesheets

Exercises:
*	https://flukeout.github.io/

Reference websites:
*	https://css-tricks.com/
*	https://www.supremo.co.uk/typeterms/
*	https://css-tricks.com/snippets/css/a-guide-to-flexbox/
*	https://unsplash.com/
* https://developer.mozilla.org/es/docs/Learn/CSS/Introduction_to_CSS/Cascada_y_herencia
*	https://specificity.keegan.st/

Website for color check:
*	http://paletton.com/
*	https://coolors.co/

Website for fonts download:
*	https://fonts.google.com/


******************************************************************************************
## 7.	__Advanced CSS__
Critical Render Path
*       When rendering a webpage, browser (client) will send requests for HTML, CSS and maybe fonts from other website, making rendering slow. Thus, you can use CSS minifying tool to make your CSS file small. 

Flexbox (Make image looks better. Ref: http://flexboxfroggy.com/, cheetsheet: https://darekkay.com/dev/flexbox-cheatsheet.html)
*	`display: flex`
*	`flex-direction`
*	`flex-wrap`
*	`flex-flow`
*	`justify-content`
*	`align-items`
*	`align-content`
*	`order`
*	`flex`: `flex-grow`, `flex-shrink` and `flex-basis`
*	`align-self`

Properties (by using transforma and transitions, we can make dynamic interactions)
```
	img{
		width: 450px;
		height: 300px;
		margin: 10px;
		transition: all 1s;
	}
	
	img:hover{
		transform: scale(1.1);
	}
```
*	`transition` : i.e. `all 1s` 
*	`transform` : i.e. `scale(1.1)`
*	`box-shadow`

Tools
*	Chrome Toggle Device
*	https://codepen.io/

Exercises:


Reference websites:
*	https://caniuse.com/
*	https://www.w3schools.com/cssref/css3_browsersupport.asp
*	http://shouldiprefix.com/
*	https://robots.thoughtbot.com/transitions-and-transforms

> __If you take one thing from this, it is this__: Don't worry if you don't feel 100% confident in CSS. Keep going as we will keep building on top of this knowledge.

******************************************************************************************
## 8.	__Bootstrap 4, Templates, And Building Your Startup Landing Page__


App for creating users list:
*	https://mailchimp.com


Website with animation examples:
*	https://daneden.github.io/animate.css

Website for patterns:
*	https://www.creative-tim.com/bootstrap-themes/ui-kit?direction=asc&sort=price
*	http://mashup-template.com/templates.html
*	https://startbootstrap.com/template-categories/all/
*	https://mdbootstrap.com/freebies/
*	https://www.creative-tim.com/


Generating animated patterns:
*	https://daneden.github.io/animate.css/


Installing Github:
*	https://desktop.github.com/

******************************************************************************************
## 9.	__CSS Grid + CSS Layout__

Grid Cheat Sheet:
*	http://grid.malven.co/

Grid Garden:
*	https://cssgridgarden.com/

Free Design resources:
*	https://interfacer.xyz/

******************************************************************************************
## 10.	__Career Of A Web Developer__
******************************************************************************************

******************************************************************************************
## 11.	__Javascript__
******************************************************************************************

******************************************************************************************
## 12.	__DOM Manipulation__



Reference websites:
*	https://developer.mozilla.org/en-US/docs/web/Events
*	https://www.cambiaresearch.com/articles/15/javascript-char-codes-key-codes
*	https://jquery.com/
*	http://youmightnotneedjquery.com/
*	https://babeljs.io/

******************************************************************************************
## 13.	__Advanced Javascript__
******************************************************************************************

******************************************************************************************
## 14. __Command Line__



FOR MAC OR LINUX:


Command | Description
--- | ---
ls  | lists files and folders within working directory
pwd | show current working directory
cd  | change working directory to user directory
cd .. | change working directory to direct parent directory
clear | clear current terminal screen
cd / | change current directory to root directory
cd ~ | change current directory to user directory
cd path/to/folder | changes working directory to specified path
mkdir name | create folder called 'name' within current directory
open foldername | opens folder called 'foldername' using OS GUI
touch index.html | creates new file titled index.html within working directory
open  index.html | opens file named index.html using default system program
open -a “Sublime Text” | opens sublime text program. This syntax can be used to open other programs
open . | opens and displays current folder within OS GUI
mv index.html about.html | renames index.html file to about.html
up and down arrow | cycles through previous commands typed within current terminal session
rm filename | deletes a file called 'filename' within the current directory
rm -r foldername | used to delete folders. In this case 'foldername' will be deleted
say hello (only on Mac) | the mac will speak any text you enter after the 'say' keyword


FOR WINDOWS:


```cmd
dir - list files
cd {directory name} - change directory
cd / - go to root (top) directory
cd .. - go up a level
mkdir {file name} - make a directory
echo > {filename} - create an empty file
del {filename} - remove a file
rmdir {directory name} - remove a directory and all files within
rename {filename} {new filename} - rename a file or folder
start {filename} - open file in default program
start . - open current directory
cls - clear the terminal screen
```


******************************************************************************************
## 15.	__Developer Environment__

Popular code editors:
* [Sublime Text 3](https://www.sublimetext.com/3)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Atom](https://atom.io/)

******************************************************************************************
## 16.	__Git + Github + Open Source Projects__



Install Git:
*	https://www.atlassian.com/git/tutorials/install-git#windows
*	https://www.atlassian.com/git/tutorials/install-git


```
git clone “https:……”
git status
git add “filename”
git add .
git commit –m”message”
git push
git pull
git branch
git branch “name”
git checkout “name”
git merge “name”
```


Once you are in your forked project directory in your command prompt....



1.	Type git remote -v and press Enter. You'll see the current configured remote repository for your fork.

	a.	```git remote -v```


	b.	```origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)```


	c.	```origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)```


2.	Type git remote add upstream, and then paste the URL you would copy from the original repository if you were to do a git clone. Press Enter. It will look like this:


	```
	git remote add upstream https://github.com/zero-to-mastery/PROJECT_NAME.git
	```


3.	To verify the new upstream repository you've specified for your fork, type ```git remote -v``` again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.


4.	Now, you can keep your fork synced with the upstream repository with a few Git commands.
	One simple way is to do the below command from the master of your forked repository:
```git pull upstream master```

******************************************************************************************
## 17.	__A Day In The Life Of A Developer__
******************************************************************************************

******************************************************************************************
## 18.	__NPM + NPM Scripts__


```
npm init
npm install
npm install –g browserify
```

Install node and npm:
*	https://www.npmjs.com/get-npm
*	https://nodejs.org/es/

Reference websites:
*	https://www.npmjs.com/
*	https://www.npmjs.com/package/react
*	https://lodash.com/

******************************************************************************************
## 19.	__React.js + Redux__

```
npm install –g create-react-app
create-react-app “name”
npm start
npm install tachyons
```


Website for fonts download:
*	http://www.cufonfonts.com/en


Reference websites:
*	https://reactjs.org/docs/react-component.html
*	https://jsonplaceholder.typicode.com/
*	http://atomicdesign.bradfrost.com/
*	https://robohash.org

Action --> Reducer --> Store --> Make changes

```
npm install redux
npm install react-redux
npm install redux-logger
npm install redux-thunk
```


*	https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en
*	https://reacttraining.com/react-router/
*	https://ramdajs.com/
*	https://lodash.com
*	https://glamorous.rocks
*	https://www.styled-components.com
*	https://github.com/css-modules/css-modules
*	https://www.gatsbyjs.org
*	https://zeit.co/blog/next5
*	www.material-ui.com/#/components/app-bar
*	https://react.semantic-ui.com/elements/button
*	https://github.com/reactjs/reselect
*	https://redux-saga.js.org
*	https://facebook.github.io/immutable-js/

******************************************************************************************
## 20.	__HTTP/JSON/AJAX + Asynchronous Javascript__
******************************************************************************************

******************************************************************************************
## 21.	__Backend Basics__
******************************************************************************************

******************************************************************************************
## 22. __APIs__
******************************************************************************************
*	https://stripe.com/docs/api
*	https://www.twilio.com/docs/api/messaging/send-messages
*	https://apilist.fun


******************************************************************************************
## 23.	__FINAL PROJECT: SmartBrain Front-End__


Animated objects library:
*	https://www.npmjs.com/package/react-tilt
	```
	npm install –save react-tilt
	```

Background patterns:
*	http://lea.verou.me/css3patterns/


Animated background library:
*	https://vincentgarreau.com/particles.js/

	```
	npm install react-particles-js
	```

Image and video recognition:
*	https://clarifai.com/developer/guide/
	```
	npm install clarifai
	```
Icons library:
*	https://icons8.com/icon

******************************************************************************************
## 24.	__Node.js + Express.js__

Install Postman:
*	https://www.getpostman.com/apps

Express.js:
*	https://expressjs.com/en/api.html

(Getting start guide)

```
npm install body-parser
npm install express --save
npm install --save-dev nodemon
```

Node.js Reference websites:
*	https://nodejs.org/en/
*	https://nodejs.org/api/modules.html

Storing passwords securely:
```
npm install bcrypt-nodejs
```
*	https://www.npmjs.com/package/bcrypt-nodejs
*	https://www.npmjs.com/package/argon2


```
$ npm install bcrypt
```

```jsx
1.	/*
2.	* You can copy and run the code below to play around with bcrypt
3.	* However this is for demonstration purposes only. Use these concepts
4.	* to adapt to your own project needs.
5.	*/
6.
7.	import bcrypt from'bcrypt'
8.	const saltRounds = 10 // increase this if you want more iterations
9.	const userPassword = 'supersecretpassword'
10.	const randomPassword = 'fakepassword'
11.
12.	const storeUserPassword = (password, salt) =>
13.	  bcrypt.hash(password, salt).then(storeHashInDatabase)
14.
15.	const storeHashInDatabase = (hash) => {
16.	   // Store the hash in your password DB
17.	   return hash // For now we are returning the hash for testing at the bottom
18.	}
19.
20.	// Returns true if user password is correct, returns false otherwise
21.	const checkUserPassword = (enteredPassword, storedPasswordHash) =>
22.	  bcrypt.compare(enteredPassword, storedPasswordHash)
23.
24.
25.	// This is for demonstration purposes only.
26.	storeUserPassword(userPassword, saltRounds)
27.	  .then(hash =>
28.	    // change param userPassword to randomPassword to get false
29.	    checkUserPassword(userPassword, hash)
30.	  )
31.	  .then(console.log)
32.	  .catch(console.error)
```


******************************************************************************************
## 25.	__FINAL PROJECT: SmartBrain Back-End -- Server__


Change localhost:
*	https://stackoverflow.com/questions/40714583/how-to-specify-a-port-to-run-a-create-react-app-based-project

If you don't want set environment variable, other option - modify scripts part of package.json from:

```"start": "react-scripts start"```

Linux (tested on Ubuntu 14.04/16.04) and MacOS (tested by @aswin-s on MacOS Sierra 10.12.4) to:

```"start": "PORT=3006 react-scripts start"```

or (maybe) more general solution by @IsaacPak to:

```"start": "export PORT=3006 react-scripts start"```

Windows @JacobEnsor solution to:

```"start": "set PORT=3006 && react-scripts start"```


Front-end and back-end connection:
*	https://www.npmjs.com/package/cors
	```
	npm install cors
	```

Front-end:

```Javascript
fetch('http://localhost:3000/image', {
	method: 'put',
	headers: {'Content-Type': 'application/json'},
	body: JSON.stringify({
		id: this.state.user.id
	})
})
.then(response => response.json())
.then(count => {
	this.setState(Object.assign(this.state.user, { entries:count}))
})
```
Back-end:

```Javascript
const cors = require('cors')
app.use(cors());
```

******************************************************************************************
## 26.	__Databases__


Install PostgreSQL:

*	http://www.psequel.com/

	en el terminal:
	```zsh
	brew update
	brew doctor
	brew install postgresql
	brew services start postgresql
	brew services stop postgresql
	createdb ‘test’
	psql ‘test’
	```

	for windows:

*	https://www.pgadmin.org/download/pgadmin-4-windows/
*	http://www.postgresqltutorial.com/install-postgresql/

	```cmd
	@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('https://s3.amazonaws.com/pgcentral/install.ps1'))"

	cd bigsql
	pgc install pg10
	pgc start pg10
	```
*	http://dc-apuntes.blogspot.com/2016/04/comandos-postgres-desde-cmd-windows.html
*	https://www.w3resource.com/PostgreSQL/connect-to-postgresql-database.php
*	https://www.youtube.com/watch?v=fD7x8hd9yE4

data types
*	https://www.techonthenet.com/postgresql/datatypes.php

Terminal commands for windows:

Login: (-U usuario)

	psql -h localhost -U postgres

Create database:

	create database database_name;

Show all datatables:

	\l

Create a user:

	create user moni with password ‘moni’;

Delete a database:

	drop database database_name;

Connect to a database:

	\c database_name;

Create a schema:

	create schema friends;

Create a table:

	create table Friends.test( firstname CHAR(15), lastname CHAR(20));

	create table Friends.login(id serial not null primary key, secret varchar (100) not null, name text unique not null, entries bigint default 0, joined timestamp not null);

Show all information of a table:

	select * from friends.test;

Describe database:

	\d friends.test

Insert data:

	insert into friends.test values( ‘Mike’, ‘Smith’);

	insert into friends.test (firstname, lastname )values( ‘Sally’, ‘Jones’);

Add a column to an existing table:

	alter table Friends.test add age smallint;

Update data from the table:

	update friends.test set age = 25 where firstname= ‘Mike’;

Delete data from the table:

	delete from friends.test where firstname = ‘Mike’;

Delete column from a table:

	alter table friends.test drop column age;

Delete a table:

	drop table friends.test;

Functions:

	select avg(age) from friends.test;

Join tables:

	select * from friends.test join friends.login on friends.test.firstname = friends.login.name;

Exit:

	\q

List all users in postgresSQL database server:

	\du

List all tables in a schema:

	\d+ schema_name.*

List all tables in a database:

	\dt *.*

List a table in a schema:

	\d+ schema_name . table_name

Show description of a table, columns, type, modifications, etc.:

	\d+ table_name

Create a backup of a database:

	pg_dump -h localhost -U postgres database_name > database_name.sql

Restore a database: 1. Create a new database where the restore file is going to be placed:

	psql -U postgres -d new_database_name -f respaldo.sql

	*Note:  it is important to create the restore in the same root where the database copy is saved.

Enter to postgres with a user different to postgres:

	psql -h localhost -d postgres -U usuario

Enter to a database with a different user:

	psql -h localhost -d nombre_base -U nombre_usuario


******************************************************************************************
## 27.	__FINAL PROJECT: SmartBrain Back-End – Database__


Tool for db connection with back-end:
*	https://knexjs.org/
*	https://knexjs.org/#Installation-node
*	https://github.com/vitaly-t/pg-promise

******************************************************************************************
## 28.	__Production + Deployment__


Environmental variables:
*	http://www.dowdandassociates.com/blog/content/howto-set-an-environment-variable-in-windows-command-line-and-registry/

### PORT

On terminal:

	bash
	-->PORT-3000 node server.js

On server.js:
```JSX
	const PORT = process.env.PORT
	app.listen(PORT, ()=>{
		console.log(`app is running on port ${PORT}`);
	})
```

### DATABASE

On terminal:

	bash
	-->DATABASE_URL-123  node server.js

On server.js:

```jsx
	const DATABASE_URL = process.env. DATABASE_URL
	app.listen(3000, ()=>{
		console.log(`app is running on port ${ DATABASE_URL }`);
	})
```

### OTHER OPTION

On terminal:

	fish
	-->env DATABASE_URL-‘hello’ node server.js

Deploy apps:

Heroku:

*	https://www.heroku.com/
*	https://devcenter.heroku.com/articles/git

Not the best one:
*	https://www.hostgator.com/promo/snappy60?utm_source=google&utm_medium=brandsearch&kclickid=cfe89874-3c6a-404e-b321-fc3e56f9ec2b&gclid=CjwKCAjwsJ3ZBRBJEiwAtuvtlIkFb-qOw3HN_JpH3AAkmYwKhk_L0y0stl7J1CFRR8FRltvmvhwXPBoCATIQAvD_BwE



Commands for heroku on backend folder:
Install heroku:
```
npm install -g heroku
heroku login
heroku create
```
In the terminal there will be a URL : ” https://limitless-bastion-10041.herokuapp.com/”
```
git remote –v
git push origin master
heroku git: remote –a limitless-bastion-10041
```

Changes required in:

*	BACK END: PORT in server.js needs to be changed by an environment variable
*	FRONT END: fetch URL needs to be changed by the URL of HEROKU + “:3000”

```
git push heroku master
for checking errors:
heroku logs --tail
heroku open
```


Connect to pg database:
*	https://devcenter.heroku.com/articles/heroku-postgresql
*	https://docs.aws.amazon.com/es_es/AmazonRDS/latest/UserGuide/USER_ConnectToPostgreSQLInstance.html
*	https://msdn.microsoft.com/en-us/library/ms175043(v=sql.120).aspx#SSMSProcedure

Create a new postgres database using Heroku:

Data: Heroku postgres: create new: install heroku postgres: select the app created
```
heroku addons
heroku info
heroku pg:psql
```

******************************************************************************************
## 29.	__Where To Go From Here?__
******************************************************************************************

The Complete Junior to Senior Web Developer Roadmap (2019):
*	https://www.udemy.com/the-complete-junior-to-senior-web-developer-roadmap/

******************************************************************************************
## 30.	__Bonus: Extra Bits (Coding Challenges + AMA)__
******************************************************************************************
******************************************************************************************
## 31.	__Extra: For Windows Users__
******************************************************************************************
******************************************************************************************
## 32.	__Bonus: Part 2 - Special Thank You Gift (Discount Coupons)__
******************************************************************************************

