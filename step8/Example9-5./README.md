# Am I root?

## Description

The following scripts both have the same goal: to check if the user is root.

In the first case, the script compares the user's $UID (the user ID of the one running the script) with $ROOT_UID. If the -eq condition is true, it prints "You are root".

In the second script, the purpose is the same, but instead of comparing user IDs, it compares $ROOTUSER_NAME with $username. If they match, the user is identified as root.
