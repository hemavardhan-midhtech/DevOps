# User Management

## User Concepts

Linux uses users and groups for access control.

## Important Files

### /etc/passwd

User information.

### /etc/shadow

Encrypted passwords.

### /etc/group

Group information.

## User Commands

Create User

useradd john

Set Password

passwd john

Delete User

userdel john

Delete User with Home

userdel -r john

Modify User

usermod

## Group Commands

Create Group

groupadd devops

Add User to Group

usermod -aG devops john

Delete Group

groupdel devops

## Sudo Access

Edit:

visudo

Example:

john ALL=(ALL) NOPASSWD:ALL

## Account Information

id john

groups john

whoami

## Switch User

su -

sudo su -

## Password Aging

chage -l john

## Lab

1. Create 3 users.
2. Create DevOps group.
3. Add users to group.
4. Configure sudo access.

## Interview Questions

Q: Difference between useradd and adduser?

A: useradd is low-level; adduser is interactive.

Q: What is sudo?

A: Allows authorized users to execute commands as another user.

Q: Where are passwords stored?

A: /etc/shadow
