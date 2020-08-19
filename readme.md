## Sayed Rashid Ali Shah
## 2K18/CSM/101
<br><br><br>




# <i><u>ARTICAL 1</i></u>
# DeepSQLi: Deep Semantic Learning for Testing SQL Injection
## AUTHORS/RESEARCHERS:
<br>
1. Muyang Liu<br>
2.  Ke Li<br> 
3. Tao Chen

<br><br>
>Venue. Tue 21 Jul 2020 14:10 - 14:30 at Zoom - SECURITY 
**_Chair(s): Lucas Bang**

### <br><i>[LINK URL](https://conf.researchr.org/details/issta-2020/issta-2020-papers/9/DeepSQLi-Deep-Semantic-Learning-for-Testing-SQL-Injection)
</i><hr><br><br>
# Introduction

+ SQL injection is a code injection technique that might destroy your database.
+ SQL injection is one of the most common web hacking techniques.
+ SQL injection is the placement of malicious code in SQL statements, via web page input.

# <br><br>SQL in Web Pages
<br>
SQL injection usually occurs when you ask a user for input, like their username/userid, and instead of a name/id, the user gives you an SQL statement that you will unknowingly run on your database.
<b><br> example which creates a</b> <br>
SELECT statement by adding a variable (txtUserId) to a select string. The variable is fetched from <b><hr>user input </b>(getRequestString):
txtUserId = getRequestString("UserId");<br><br>
txtSQL = "SELECT * FROM Users WHERE UserId = " + txtUserId;


+ SQL Injection Based on 1=1 is Always True
Look at the example above again. The original purpose of the code was to create an SQL statement to select a user, with a given user id.
+ If there is nothing to prevent a user from entering "wrong" input, the user can enter some "smart" input like this:
<hr>Then, the SQL statement will look like this:
<br><br><b>SELECT * FROM Users WHERE UserId = 105 OR 1=1;</b><br><br>

+ The SQL above is valid and will return ALL rows from the "Users" table, since OR 1=1 is always TRUE.
+ Does the example above look dangerous? What if the "Users" table contains names and passwords?
+ The SQL statement above is much the same as this:
SELECT UserId, Name, Password FROM Users WHERE UserId = 105 or 1=1;
+ A hacker might get access to all the user names and passwords in a database, by simply inserting 105 OR 1=1 into the input field.

## SQL Injection Based on ""="" is Always True
Here is an example of a user login on a web site:<br><b>
uName = getRequestString("username");
<br>uPass = getRequestString("userpassword");</b>

sql = 'SELECT * FROM Users WHERE Name ="' + uName + '" AND Pass ="' + uPass + '"'
<br><br>SELECT * FROM Users WHERE Name ="John Doe" AND Pass ="myPass"
<br><br>
+ A hacker might get access to user names and passwords in a database by simply inserting " OR ""=" into the user name or password text box:
<br><br>
SELECT * FROM Users WHERE Name ="" or ""="" AND Pass ="" or ""=""
<br><br>The SQL above is valid and will return all rows from the "Users" table, since OR ""="" is always TRUE.







# <i><br><u>ARTICAL 2</i></u>


<br><br>


# <b> From Innovations to Prospects: What Is Hidden Behind Cryptocurrencies?</b>


## AUTHORS/RESEARCHERS:
1. Ang Jia
2. Xi Xu
3. Wenying Wei
4. Di Cui
5. Zijiang Yang
6. Kai ye
7. Ting liu



> Venue.Tue 30 Jun 2020 16:30 - 16:45 at MSR:Zoom2 - Visions & Reflections \
**_Chair(s): Venera Arnaoudova_** 

<br>

### [LINK URL](https://2020.msrconf.org/details/msr-2020-papers/45/From-Innovations-to-Prospects-What-Is-Hidden-Behind-Cryptocurrencies-)
<hr><br><br>




# Introduction

## <b>Cryptocurrency</b>


A cryptocurrency (or crypto currency) is a digital asset designed to work as a medium of exchange wherein individual coin ownership records are stored in a ledger existing in a form of computerized database using strong cryptography to secure transaction records, to control the creation of additional coins, and to verify the transfer of coin ownership.[1][2] It typically does not exist in physical form (like paper money) and is typically not issued by a central authority. Cryptocurrencies typically use decentralized control as opposed to centralized digital currency and central banking systems

<br>

<i><b>Bitcoin</b>, first released as open-source software in 2009, is the first decentralized cryptocurrency.[5] Since the release of bitcoin, over 6,000 altcoins (alternative variants of bitcoin, or other cryptocurrencies) have been created.
</i>



## <b>Bitcoin

>Bitcoin is a cryptocurrency invented in 2008 by an unknown person or group of people using the name Satoshi Nakamoto and started in 2009, when its implementation was released as 
(OSS) open-source software.

<i>(Open-source software (OSS) is a type of computer software in which source code is released under a license in which the copyright holder grants users the rights to use, study, change, and distribute the software to anyone and for any purpose)</i>


## <b>Altcoin

>The term altcoin has various similar definitions. Stephanie Yang of The Wall Street Journal defined altcoins as "alternative digital currencies," while Paul Vigna, also of The Wall Street Journal, described altcoins as alternative versions of bitcoin. Aaron Hankins of MarketWatch refers to any cryptocurrencies other than bitcoin as altcoins.




