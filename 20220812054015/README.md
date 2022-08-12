# Connect to a ssh remote via PEM key

1. Make ```.ssh``` in your home directroy and ```cd``` into it
```bash
mkdir ~/.ssh
chmod 700 ~/.ssh
```
2. Generate ssh key if you don't have one
```bash
ssh-keygen -t rsa -b 4096 -f <rsa_key_name> -v
```
3. Create ```authorized_keys``` file under ```~/.ssh```
```bash
touch ~/.ssh/authorized_keys
chmod 600 ~/.ssh/authorized_keys
```
4. Add the ```.pub``` file of the key you've just created to the
	 ```authorized_keys``` file
```bash
cat <rsa_key_name> >> authorized_keys
```
5. Generate ```PEM``` key
```bash
openssl rsa -in <rsa_key_name> -outform PEM -out <pem_key_name>.pem
chomd 600 <pem_key_name>.pem
```
6. [Optional] add passphrase to your pem key file
```bash
ssh-keygen -p -f <pem_key_name>
# check it the key has any passphrase
ssh-keygen -y -f <pem_key_name>
```
7. Connect to the remote machine with pem file
```bash
ssh -i <pem_key_name> <username>@<ip_address>
```
