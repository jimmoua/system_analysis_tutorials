<h1>MariaDB</h1>

**The main purpose of this guide is to only show you how to install MariaDB and nothing else**. After that you can connect to any AWS RDS that uses MySQL or MariaDB as a database.

You can read more on how to configure it [here](https://wiki.archlinux.org/index.php/MariaDB). This includes setting up new users, creating other databases, and other neat stuff.

What is MariaDB? A very short excerpt taken from Wikipedia:

> MariaDB is a community-developed, commercially supported fork of the MySQL relational database management system, intended to remain free and open-source software under the GNU General Public License.

<h1>Table of Contents</h1>

- [Installation](#installation)
  - [Windows](#windows)
  - [Linux](#linux)

# Installation

## Windows
Install it using Chocolatey package manager.

```
$ choco install mariadb
```
After installing it, you can connect to the AWS using

```
$ mariadb -h <host-endpoint> -u <username> -p
```

If you want to configure MariaDB on your local machine, the default username is `root` and the password is empty, so you can log in with these credentials on your terminal emulator:

```
$ mariadb -u root -p
```

## Linux

> Install mariadb, and run the following command before starting the `mariadb.service`:
```
# mariadb-install-db --user=mysql --basedir=/usr --datadir=/var/lib/mysql
```

Since most distributions of Linux use `systemd`, you can enable the service like so:

```
$ sudo systemctl enable mariadb.service
```

And then start it with

```
$ sudo systemctl start mariadb.service
```

Connecting is the same as shown above in Windows.