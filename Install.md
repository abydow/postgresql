1. PostgreSQL from https://www.postgresql.org/download/
2. Pgadmin 4 https://www.pgadmin.org/ (install desktop and web both version)

   > If you use fedora or any distro based on RHEL/derivatives
   > And if you install Pgadmin from command line interface

   \*\* don't forget to set the password

## password setting process

- First use>>

```zsh
sudo -u postgres psql
```

- Enter your sudo password to access PosgreSQL shell

```postgres=#
\password postgres
```

> \password to setup password and postgres is the username we will use as in pgadmin 4 "postgres" is default superuser role.

- After that type you password and confirm it

```postgres=#
\q
```

- To exit out of it

# Disclaimer

In my case, I had to download pgadmin4, pgadmin4-desktop and pgadmin4-web where as in the documentation it was said in the documentation that we only need to install the first <pgadmin4> to get both desktop and web versions.
