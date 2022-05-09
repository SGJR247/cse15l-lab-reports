# Lab Report 3 - Week 6
## By Samuel Genous Jr.

*Lab 5 Group Choice Options*

**1. Streamlining ssh Configuration**

![SSH Config File](https://user-images.githubusercontent.com/103216157/167341976-1a2650ba-4544-41a4-a8ce-944402b6af8c.png)

* Added IdentityFile line and changed Host with VSCode

![Streamlined SSH Login](https://user-images.githubusercontent.com/103216157/167342121-45611b8d-769b-43e4-a1fc-c676405f71a9.png)

* SSH command logs me into my account, using just ieng6 as my alias

![Streamlined SCP](https://user-images.githubusercontent.com/103216157/167342219-f29a11c0-b2c1-44cf-a4c0-d00ceeab5aa6.png)

* SCP command copies file into my account, using just ieng6 as my alias


**2. Setup Github Access from ieng6**

![ieng6 SSH Keys](https://user-images.githubusercontent.com/103216157/167342491-ffa82122-f197-485c-afb1-092b61179020.png)

* Public & private keys meant for use with Github (id_rsa_github) shown in ieng6 account
* Public key for GIthub: ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQC4Po7D53D5ZDbnUsCyrqf25bClM72s03bvIVR1Xik1qDSxK2DUkF6dd4n1mqAbPfpfXvUGL4lN66E6GQAv8gr3lXKJbpAodpVlpCJKHgKXstmqveynhVRPjJY/xvICpUoHkslcWI0anofL4EIxDKbDaQrDMSvEzBFs6UhIUNDxY+gk5aetjf46S1XnAjF6F0s2eJ1jE1EfgZ0snNEhthESm0barHcHg+/r9U5U3OBOXCxc5A8RMAu6F6YzPkgC9suEqUtsajxnxkGCY2ZEm28qiMR3x7ae9+lINf6qDf2XacGbqR7Iz/1UNYVZA04djJaRHHf4xRq3xCxe6k4Cshk8a3vEYFC7ucGYMe2Dkr+IvLpE3UlKsaY1vUBd+CuxcUyIgQT6i/SJFnIkVoDlNJhjhsgYNFeZMeY3kR6GkbmredZJYPLA1KE84gtXxde3Z5LSdFDrt9a3wOoIAPozvezQcaL8Ri6DJxpdtp9YEw2TRvwJBy49TpkABF1sAFpec5k= genou@LAPTOP-K8AA5IC9

![Git Commit & Push Attempt](https://user-images.githubusercontent.com/103216157/167342838-250e9e82-cc73-4a02-9310-77f42bc21f28.png)

* Tried to do commit and push in ieng6, but commit wouldn't update for changes in markdown-parser repository and push ended up preventing me from entering Github (asks for username and password, requires personal access token)
* Link to Resulting Commit: N/A, due to aforementioned issues with ieng6 commit and push commands

**3. Copy whole directories with `scp -r`**

