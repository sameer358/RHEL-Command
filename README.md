RHEL Useful Commands

If you want to extract only the usernames from the `/etc/passwd` file, you can use various command-line tools like `awk`, `cut`, or `sed`. Here are a few examples:

Using `awk`:
```bash
awk -F: '{print $1}' /etc/passwd
```

Using `cut`:
```bash
cut -d: -f1 /etc/passwd
```

Using `sed`:
```bash
sed 's/:.*//' /etc/passwd
```

All these commands essentially split each line of the `/etc/passwd` file by the `:` delimiter and extract the first field, which corresponds to the username. So, you'll get a list of usernames as output. Choose the one that suits your preference or the one you're most comfortable with.
