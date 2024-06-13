# This project has been discontinued.

**When installing, keep in mind that support is not provided by this library.**

Its de facto successor library is [misspy](https://github.com/misspy-dev/misspy).
## Why was it discontinued?
Partly because the name is very similar to existing libraries such as MiPA and MiPAC, but the most important reason is that I started developing [misspy](https://github.com/misspy-dev/misspy), the spiritual successor library to MiPC.
## I want to use the PyPI project name (misskey-python) for another project, so I want to transfer it / I want to maintain MiPC, so I want to transfer the PyPI project name.
I will gladly transfer both. To request a transfer, please send an email with the reason and a repository such as GitHub. Please note that, as with PEP 541 requests, we will not respond to requests **without a valid reason**. Also, there may be a delay in confirming your email.

Please use the email address listed in the latest release when submitting, as the email addresses posted in the past are no longer in use.

# MiPC

![img](assets/icon.png)

MiPC (Misskey Python Client) is a Python client for using MisskeyAPI.

# Examples

##  MiAuth

```python

from MiPC.MiAuth import MiAuth

mia = MiAuth(server="misskey.io", name="TestApp")

url = mia.generate_url()

while True:

   try:

     auth_token = mia.get_token()

     break

   except MisskeyMiAuthFailedException:

     await asyncio.sleep(0.5)

     pass

```

# question
## Q. Why is the pypi registered under a different name(misskey-python) than MiPC?
A. Because the registration was denied due to the name being similar to an existing pypi project.
