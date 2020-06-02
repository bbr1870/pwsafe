PasswordSafe non-Windows release 1.11
=====================================

 * Fix an issue with the width of spinbox controlsi n several versions of GTK3 which causes
   spinbox controls to be displayed incorrectly - too wide or too narrow.
   In addition to some heuristics based on the distribution type and version, we allow
   the user control of the width of the spinbox via the PWS_FIX_GTK_SPINBOX environment variable as follows:
   ** 0 - This is the same as not setting the environment variable, i.e., let PasswordSafe try to determine the correct width
   ** 1 - This lets wx set the width to wxDefaultSize, which may be way too wide for some versions of GTK
   ** 2..10 - This sets the width to display this many characters in the text entry field of the spinner.

Password Safe 3.52 Release April 2020
=====================================

This note describes the new features, fixed bugs and known problems
with the latest versions of Password Safe. For a short description of
Password Safe, please see the accompanying README.md file. For more
information on the product and the project, please visit
https://pwsafe.org/. Details about changes to older
releases may be found in the file ChangeLog.txt.

In the following, SFxxxx refers to Bug Reports, Feature Requests and Service Requests in PasswordSafe SourceForge Project tickets, and GHxxxx refers to issues in the PasswordSafe GitHub project.

Bugs Fixed in 3.52
------------------
* [SF1510](https://sourceforge.net/p/passwordsafe/bugs/1510) Fixed truncated text in delete confirmation window.
* [SF1509](https://sourceforge.net/p/passwordsafe/bugs/1509) Cancelling a delete now leaves the selection unchanged.
* [GH634](https://github.com/pwsafe/pwsafe/issues/634), [SF1508](https://sourceforge.net/p/passwordsafe/bugs/1508) Clearing an entry's username no longer causes a revert to default.
* [SF1505](https://sourceforge.net/p/passwordsafe/bugs/1505) No longer crashes when trying to view or copy a shortcut from the "compare databases" results.
* [SF1503](https://sourceforge.net/p/passwordsafe/bugs/1503), [SF1512](https://sourceforge.net/p/passwordsafe/bugs/1512) Recurring password expiration update fixed ([1497](https://sourceforge.net/p/passwordsafe/bugs/1497) redo).
* [SF1495](https://sourceforge.net/p/passwordsafe/bugs/1495) Accepts policy name via Enter as well as click on OK.

