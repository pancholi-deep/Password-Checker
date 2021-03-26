this is a password checker to check how many times your password has been hacked on the internet.
steps that this code follows:
1. run this file using command "python passcheck.py 'your_password'"
2. it takes your_password, converts it into SHA-1 Hash
3. it calls the password api from 'pwnedpasswords.com' using the first 5 characters of generated SHA-1 value.
4. it gets compromised states of all passwords starting with the first 5 characters of our password from the API.(steps 3,4 are to make sure we do not call the API with our exact password or its SHA-1 value.)
5. from the API results, it finds the count of our password being hacked or not, and shows it to user.

NOTE: we could have used the pwnedpasswords website for this purpose, but it will not be safe as you will have to type in your password on that website. instead, using this tool, we will have our password only till our machine and will not be sent anywhere on the internet beyond that.