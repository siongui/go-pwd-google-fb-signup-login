================================================
Go Signup Login (Email&Password/Google/Facebook)
================================================

.. image:: https://img.shields.io/badge/Language-Go-blue.svg
   :target: https://golang.org/

.. image:: https://godoc.org/github.com/siongui/go-pwd-google-fb-signup-login?status.svg
   :target: https://godoc.org/github.com/siongui/go-pwd-google-fb-signup-login

.. image:: https://github.com/siongui/go-pwd-google-fb-signup-login/workflows/ci/badge.svg
    :target: https://github.com/siongui/go-pwd-google-fb-signup-login/blob/master/.github/workflows/ci.yml

.. image:: https://goreportcard.com/badge/github.com/siongui/go-pwd-google-fb-signup-login
   :target: https://goreportcard.com/report/github.com/siongui/go-pwd-google-fb-signup-login

.. image:: https://img.shields.io/badge/license-Unlicense-blue.svg
   :target: https://github.com/siongui/go-pwd-google-fb-signup-login/blob/master/UNLICENSE


Back-End Exam
+++++++++++++


What We Look For
----------------

This exam is designed to test if you can:

1. Follow simple, written, English instructions.
2. Build a simple sign up/sign in app that exists in all apps.
3. Find and use third party APIs to save time.
4. Write clean and well documented code.
5. Work with ambiguity in instructions to build an app that has a good user
   experience.


Requirements
------------

Create a simple app where users can sign up and sign in from a landing page into
a simple dashboard. The landing page can be blank with only two separate links
to “Sign Up” and “Sign In”. The simple dashboard can only be accessed after the
user signs up or signs in.

You may use the following tech stacks:

1. JavaScript, Node.js
2. Python, Django Rest Framework (DRF) or Fast API


Sign Up [20 points]
-------------------

The Sign Up page should allow users 3 options to create an account:

(1) email and user defined password
(2) Google OAuth
(3) Facebook OAuth

You can use any third party tool, library, or API for this. In fact, to save
time, it is highly recommended that you use a third party auth API. Create your
own guest or trial accounts with third party tools. We only need a live demo app
to test for 1 or 2 weeks.


User Defined Password [20 points]
---------------------------------

The user defined password must be entered twice and match. In addition, the
password must be validated by the following conditions.

- contains at least one lower character
- contains at least one upper character
- contains at least one digit character
- contains at least one special character
- contains at least 8 characters


Email Verification [40 points]
------------------------------

For the user defined password, after the validated password is entered, your
back-end app must send an verification email to the email address provided. The
email must contain a link, that if the user clicks the link, their email will be
verified in the back-end and the user will be directed to a simple dashboard in
a new browser.

Only accounts that have email verified can access the simple dashboard. Users
that have not verified email will only see a button or link that says “Resend
Email Verification”, and clicking on this link will resend the same email
verification.

Only accounts created via email and password must be verified with email
verification. Facebook and Google OAuth sign up accounts do not need to send
email verification, and can immediately access the simple dashboard.

Like with authentication, you can use any third party email sending tool,
library, or API. Create your own guest or trial accounts. We only need a live
demo app to test for 1 or 2 weeks.


Login [10 points]
-----------------

We will allow users to login through the 3 methods that users can sign up with:

(1) email and user defined password
(2) Google OAuth
(3) Facebook OAuth

You can use any third party tool, library, or API for this feature.


Simple Dashboard [20 points]
----------------------------

The simple dashboard will display the user’s email and name (from Google or
Facebook OAuth). In addition, the user can reset their name. Everytime the user
logins, the user should see the name they have chosen.


Reset Password [30 points]
--------------------------

In the simple dashboard, add the ability to reset password. The password must
meet the same criterias as defined previously. In addition, the user must enter
3 text input boxes:

1. Old password
2. New password
3. Re-enter new password


Development Environment
+++++++++++++++++++++++

  - `Ubuntu 20.04`_
  - `Go 1.17.1`_


UNLICENSE
+++++++++

Released in public domain. See UNLICENSE_.


References
++++++++++

.. [1] | `golang google facebook sign in - Google search <https://www.google.com/search?q=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - DuckDuckGo search <https://duckduckgo.com/?q=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Ecosia search <https://www.ecosia.org/search?q=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Qwant search <https://www.qwant.com/?q=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Bing search <https://www.bing.com/search?q=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Yahoo search <https://search.yahoo.com/search?p=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Baidu search <https://www.baidu.com/s?wd=golang+google+facebook+sign+in>`_
       | `golang google facebook sign in - Yandex search <https://www.yandex.com/search/?text=golang+google+facebook+sign+in>`_

.. [2] `How to Implement Password Authentication and Storage in Go (Golang) <https://www.sohamkamani.com/golang/password-authentication-and-storage/>`_

.. [3] `Authentication and OAuth - Awesome Go <https://github.com/avelino/awesome-go#authentication-and-oauth>`_

.. _Go: https://golang.org/
.. _Ubuntu 20.04: https://releases.ubuntu.com/20.04/
.. _Go 1.17.1: https://golang.org/dl/
.. _UNLICENSE: https://unlicense.org/
