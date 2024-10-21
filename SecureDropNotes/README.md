Project revolves around creating a secure file sharing utility operating through the command line known as "SecureDrop," with executable secure_drop.

SecureDrop will be used to, as previously mentioned, securely transfer a file to another user on the primary user's contact list and with both users on the same network.

**Due Dates:**
Milestones 1-3: 14 Nov
Milestones 4-5: 15 Dec

Sample output given from 'project.pdf':

```
# The secure_drop command serves as the entry point for the application. If no 
# user exists, the registration module will activate, with the email address 
# serving as user identifier.

$ secure_drop
No users are registered with this client.
Do you want to register a new user (y/n)? y
Enter Full Name: John Doe
Enter Email Address: john.doe@gmail.com
Enter Password: *********
Re-enter Password: *********
Passwords Match.
User Registered.
Exiting SecureDrop.
$

# The user registration is a one-time process. Once a user is registered on a 
# client, the login module is subsequently activated. After a successful login, a 
# "secure_drop>" shell is initiated.

$ secure_drop
Enter Email Address: john.doe@gmail.com
Enter Password: ****
Email and Password Combination Invalid.
Enter Email Address: john.doe@gmail.com
Enter Password: *********
Welcome to SecureDrop.
Type "help" For Commands.
secure_drop> help
"add" -> Add a new contact
"list" -> List all online contacts
"send" -> Transfer file to contact
"exit" -> Exit SecureDrop
secure_drop>

# The "add" command adds a new contact for the user. If a contact already exists, 
# it overwrites the existing details. Note that the email address is used as user # identifier.

secure_drop> add
Enter Full Name: Alice
Enter Email Address: alice@gmail.com
Contact Added.
secure_drop> add
Enter Full Name: Bob
Enter Email Address: bob@gmail.com
Contact Added.
secure_drop>

# The "list" command displays only those contacts that meet specific criteria:
# 1. The contact email is in this user's contacts.
# 2. The contact has also added this user's email to their contacts.
# 3. The contact is online on the same network.
secure_drop> list
The following contacts are online:
* Bob <bob@gmail.com>
secure_drop>

# The "send" command transfers a file to the contact. The contact must receive an
# alert and approve the transfer. You can save the file to a directory of your 
# choice, using the same file name as the transmitted file.
# Contact 'John Doe <john.doe@gmail.com>' is sending a file. Accept (y/n)?

secure_drop> send bob@gmail.com /home/john/Documents/bob.zip
Contact has accepted the transfer request.
File has been successfully transferred.
secure_drop> exit
$
```
