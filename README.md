REPLACED FOR ME
===============

I wrote this tool to keep track of unplanned things I did without having to do `task add X` and then `task done <id>` every time.
However, today @bowlofeggs pointed me to `task log`, which basically replaces it.

Feel free to continue using it, but I'll stop using it in favor of `task log`.



I Did
=====

This is a very small tool that helps with quickly recording what you did
during a period of time, without getting in the way or requiring a lot of
work.


Requirements
------------
python 2 or 3


Installation
------------
Clone the repository.
You might want to add the clone to your PATH to make it easier to execute.


Usage
-----
Default usage is just ./idid <item title> to add a new item with "<item title>" as title.

Example: ./idid Just wrote this small tool idid

Note that quotes are not needed if you use multiple arguments: it tries not to get in the way.

If you accidentally made a typo or made another mistake, run "./idid remove-last" to remove
the last entry that was added.

When you want an overview of what you did so far, just run the export command: ./idid export.
This will print out a per-day overview of entries recorded, and record the entries it has already
exported, so that you don't need to remember what you already exported: next time around, just
run ./idid export again, and it will omit any items already exported.
If you do not want to log this, you can add no-mark at the end of the command.
If you want to avoid idid printing a small banner, add no-banner at the end.
So to get a non-marked export without banner, run: "./idid export no-mark no-banner".


Ideas
-----
Feel free to submit pull requests or file issues if you have any ideas for improvement.
