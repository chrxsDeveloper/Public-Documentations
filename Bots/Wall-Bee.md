# Wall-Bee

Wall-Bee is the garbage collector bot. It checks every 2 days a specific email-inbox for orders and erases data of
databases afterwards.

## Quick-Navigation

* [How to delete data](#how-to-delete-data)
* [Body Syntax](#body-syntax)
* [Examples](#examples)
* [Contact](#contact)

## How to delete data

Send an email with the following content:

### From:

Your email address, which should be deleted

### To:

```
wall-bee@chrxsdev.de
```

### Subject:

```
[Data Deletion]
```

### Body:

If you want to erase your data of the entire system, lease the email body empty. If you want to only erase your data of
specific databases, look up the chapter [Body Syntax](#body-syntax).

## Body Syntax

Your email address is probably stored in a database, because we are working together on a project or you're using any of
my paid services and I'm sharing my password with you. So most probably you're looking this up, because you got a email
about the password rotation. If yes, follow the next steps. If not, please contact me directly, because there's no way
you know how I name my services or databases.

### Auto-generate erase order:

1. Please look up the email about the password rotation you got from [BeeMO](https://github.com/chrxsDeveloper/BeeMO).
2. At the end of the email is a clickable link, which generates a valid email, to erase your data of the
   specific database.

### Custom erase order:

1. Please look up the email about the password rotation you got from [BeeMO](https://github.com/chrxsDeveloper/BeeMO).
2. After the first paragraph is a field named `service-id`. Copy the `service-id`.
3. Open a new email and set [from](#from), [to](#to) and [subject](#subject) as described above.
4. Paste the `service-id` into the email body. If you want to erase your data of multiple databases, please separate
   them with a `,`.
5. If you want to erase your data of the entire system, expect of a specific database, please add a `!` in front of the
   `service-id`.

### Examples

The examples only show the email body. Please set [from](#from), [to](#to) and [subject](#subject) as described above.

#### Erase data of service _Spotify_ and _Disney+_

Service-IDs:

* Spotify: `spotify`
* Disney+: `disney-plus`

```
spotify, disney-plus
```

#### Erase data of entire system, expect of service _Spotify_ and _Disney+_

Service-IDs:

* Spotify: `spotify`
* Disney+: `disney-plus`

```
!spotify, !disney-plus
```

## Contact

If you have any questions, please contact me directly.

```
chrxsdeveloper@gmail.com
```