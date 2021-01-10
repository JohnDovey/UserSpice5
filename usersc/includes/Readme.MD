# UserSpice 5

## Folder: usersc/include 
---

### analytics.php
---

- Paste your analytics script at the bottom of the file.
- Don't forget your ```<script></script>``` tags!

### custom_functions.php
---

- Put your custom functions in this file and they will be automatically included.
- Use this statement during debugging to see that your custom functions are being included: 

```php
bold("<br><br>custom helpers included");
```

### database_navigation_hooks_dropdown.php
---

- Include your custom dropdown hooks here! Examples:

```php 
$dropdownString = str_replace('{{lname}}',$user->data()->lname,$dropdownString);
```

```php
$dropdownString = str_replace('{{home}}',lang("MENU_HOME"),$dropdownString);
```

### database_navigation_hooks.php
---

- Include your custom hooks here! Examples: 
```php
$itemString = str_replace('{{lname}}',$user->data()->lname,$itemString);
```
### footer.php
---

- This will go in **every** template.

### head_tags.php
---

- Facebook sharing meta tags *(delete if you don't want them)*
- <mark>Be sure to update this in .11</mark> 

```php
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
<meta name="description" content="">
<meta name="author" content="">
<meta property="og:url"                content="" /> <!-- URL for website (link address) -->
<meta property="og:type"               content="website" /> <!-- type of site -->
<meta property="og:title"              content="Userspice Site" /> <!-- title of site (title of share) -->
<meta property="og:description"        content="Powered by UserSpice" /> <!-- description of site (text which appears when sharing) -->
<meta property="og:image"              content="" /> <!-- URL for preview image
```

### oauth_success_redirect.php
---

- Whatever you want to do prior to the *account.php* redirect on *oauth_success*, you can do here

### security_headers.php
---

- Feel free to edit these as desired. They're just suggestions.
- Security Headers can be scanned using https://securityheaders.io/
  - **Content Security Policy:**
    - The content-security-policy HTTP header provides an additional layer of security. This policy helps prevent attacks such as Cross Site Scripting (XSS) and other code injection attacks by defining content sources which are approved and thus allowing the browser to load them.
  - Not specified because you cannot predict what content sources will be required by the users of UserSpice **

### user_agreement.php
---

Welcome to our website. If you continue to browse and use this website, you are agreeing to comply with and be bound by the following terms and conditions of use, which together with our privacy policy govern our relationship with you in relation to this website. If you disagree with any part of these terms and conditions, please do not use our website.

The use of this website is subject to the following terms of use:
- The content of the pages of this website is for your general information and use only. It is subject to change without notice.
- This website uses cookies to monitor browsing preferences. If you do allow cookies to be used, the following personal information may be stored by us for use by third parties.
- Neither we nor any third parties provide any warranty or guarantee as to the accuracy, timeliness, performance, completeness or suitability of the information and materials found or offered on this website for any particular purpose.

### UserSpice version

```php
$user_spice_ver = '5.2.1';
```
---

> ## UserSpice 5
> An Open Source PHP User Management System
> by the UserSpice Team at http://UserSpice.com
