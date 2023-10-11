# Wall-Bee

Wall-Bee is the garbage collector bot. It checks every 2 days a specific email-inbox for orders and erases data of
databases afterwards.

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

