# 2xx

php/mysql steps to the inside-out-project

<https://2xx.tylerblood.com>

<https://tyler-blood.github.io/2xx/>

***

<details><summary>Version 200.0</summary>

- pulled files from client's HTML site and uploaded to dev server.
- updated title tag and header title with PHP variable
- converted all HTML comments to PHP comments

</details>

<details><summary>Version 201.0</summary>

- replaced top level pages by changing them to php files (love who, challenges, you)
- removed header and footer from the pages replaced
- created the include folder
- created the header.inc.php and footer.inc.php files

</details>

<details><summary>Version 202.0</summary>

- replaced navigation menu with top level pages by creating a function and array to dynamically create the menu (love who, challenges, you)
- created the functions.inc.php file
  - created the menuBuilder function
  - created the menu.data.php file
  - created menuItems array
  - included in the very top of the header.inc.php a require_once to the include/menu.data.php file
- included in the very top of the header.inc.php a require_once to the include/functions.inc.php file

</details>

<details><summary>Version 203.0</summary>

- rename the menu.data.php page to content.data.php and made updates in header.inc.php
  - make modifications to the content.data.php page
    - change the variable/array name from "$menuItems" to "$content"
    - replace all instances of "MenuLink" with "pageLink"
    - replace all instances of "MenuName" with "pageName"
    - add the "childPages" sub-array for each of the pages
  - updated the menuBuilder() function to recursivly handle child data
  - created a config.inc.php file to keep our global variables in as we create them.
  - Added the code to the footer.inc.php page to add the copyright and version information.
  - Added class to the style.css page for the copyright and version. (.copyright)
  - Added redirect to force a secure connection in the header.inc.php.

</details>

<details><summary>Version 204.0</summary>

- replaced html in header.inc and footer.inc.php files with responsive bootstrap html
- updated the menuBuilder() function to bypass the homepage when building the menu
- added the getPages function to the functions.inc.php file
- added the constant variable "DEFAULT_PAGE" to establish the default page
- updated the constant variable "VERSION" to 2.0.4.0
- put the getPage function in the index.php page
- added pageContent to the content array
- added the following files:
  - assets/css/animate.min.css
  - assets/css/bootstrap.css
  - assets/css/style.css
  - assets/js/app.js
  - assets/js/html5shiv.min.js
  - assets/js/bootstrap.js
  - assets/js/jquery-1.11.3.min.js
  - assets/js/respond.min.js

</details>
