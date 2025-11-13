# OPEN-SOURCE-EX-3
# NAME:MADHANRAJ P
# REG NO:212223220052
# Aim:

To create a group named admin, add users harry and natasha to the group as secondary members, create a user sarah without interactive shell access, and set passwords for all three users in Red Hat Enterprise Linux.

# Algorithm:
<H2>Step 1:</H2>
Start the Terminal.
Open the terminal in the Red Hat Linux environment with administrative privileges.
<h2>Step 2:</h2>
Create a New Group.
Create a group named admin to manage administrative users.
<h2>Step 3:</h2>
Create User Accounts with Group Assignments.
Add a user named harry and make admin his secondary group.
Add another user named natasha with admin as her secondary group as well.
<h2>Step 4:</h2>
Create a User Without Shell Access.
Create a user named sarah who should not have access to an interactive shell (assign /sbin/nologin as the shell).
She should not be a member of the admin group.
<h2>Step 5</h2>
Assign Passwords to All Users.
Set the password redhat for users harry, natasha, and sarah.
<h2>Step 6:</h2>
Verify Group Memberships.
Display the groups of each user to confirm the correct group assignments.
<h2>Step 7:</h2>
Verify Non-Interactive Shell Access.
Check the user details of sarah in the /etc/passwd file to confirm that the shell is set to /sbin/nologin.

# Steps Involved:
```
STEP 1 : sudo groupadd admin
STEP 2 : sudo useradd -m -G admin harry
STEP 3 : sudo useradd -m -G admin natasha
STEP 4 : sudo useradd -m -s /sbin/nologin sarah
STEP 5 : echo "harry:redhat" | sudo chpasswd
          echo "natasha:redhat" | sudo chpasswd
          echo "sarah:redhat" | sudo chpasswd
STEP 6 : groups harry
          groups natasha
          groups sarah
STEP 7 : grep sarah /etc/passwd
```
# Output:
<img width="907" height="604" alt="image" src="https://github.com/user-attachments/assets/9816be47-9cb6-4a9d-a8bc-19ccc311292a" />


# Result:

Thus, the users, groups, and memberships were successfully created and verified in Red Hat Enterprise Linux using appropriate administrative commands.
