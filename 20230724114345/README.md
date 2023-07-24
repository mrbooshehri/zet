# `/bin/false` vs `/usr/bin/nologin`

Both `/bin/false` and `/usr/sbin/nologin` are commonly used as shell
replacements for user accounts that are not intended to have interactive
login access. However, there are some differences between the two:

1. **`/bin/false`:** When assigned as the shell for a user, `/bin/false`
	 simply exits immediately, returning a non-zero exit status. It does
	 not provide any error message or feedback to the user. This means
	 that users assigned `/bin/false` as their shell cannot log in at all,
	 neither interactively nor via SSH. It is typically used to create
	 "pseudo-users" or accounts that are used for specific purposes but do
	 not require login access.

2. **`/usr/sbin/nologin`:** When assigned as the shell for a user,
	 `/usr/sbin/nologin` displays a customizable error message to the user
	 attempting to log in. This message informs them that login is not
	 permitted and provides a reason for the denial. The message can be
	 configured in the `/etc/nologin.txt` file. Users assigned
	 `/usr/sbin/nologin` as their shell can still receive system
	 notifications, read mail, and perform other non-login related
	 activities. This shell is often used to restrict interactive login
	 access for system accounts or temporary account suspensions.

The choice between `/bin/false` and `/usr/sbin/nologin` depends on your
specific requirements. If you simply want to prevent a user from logging
in entirely, `/bin/false` is a lightweight option. On the other hand, if
you prefer to display a custom message explaining the login denial,
`/usr/sbin/nologin` is the recommended choice.

It's important to note that both `/bin/false` and `/usr/sbin/nologin`
should only be assigned as the shell for non-interactive accounts. They
are not suitable for regular user accounts that require interactive
login access.

To set a custom message for the `/usr/sbin/nologin` shell, you can
modify the contents of the `/etc/nologin.txt` file. This file is read by
the `nologin` program and its contents are displayed to users when they
attempt to log in using an account with `/usr/sbin/nologin` as the
assigned shell.

Follow these steps to set a custom message:

1. Open a terminal or log in as the root user.

2. Open the `/etc/nologin.txt` file using a text editor, such as `vi` or
	 `nano`: ``` sudo vi /etc/nologin.txt ```

3. Enter your desired message in the file, providing an explanation for
	 the login denial. For example: ``` Access to this account is
	 temporarily disabled for maintenance purposes. Please try again
	 later. ```

4. Save the changes and exit the text editor.

Now, when a user with `/usr/sbin/nologin` as their assigned shell
attempts to log in, they will see the custom message you defined in the
`/etc/nologin.txt` file.

Remember to use sudo or root privileges when modifying system files.

Tags:

```
#Linux #login #nologin #/bin/false #/usr/sbin/nologin #false
```
