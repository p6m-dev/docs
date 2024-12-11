### Git

## Git Installation
[https://git-scm.com/downloads](https://git-scm.com/downloads)

```sh
git --version
```

## SSH Key Generation
```sh
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## Add SSH Key to your GitHub account
1. Copy public key
```sh
cat ~\.ssh\id_rsa.pub
```
2. Go to [https://github.com](https://github.com)
3. Login to your account
4. Go Profile → Settings → SSH and GPG Keys → New SSH key
5. Paste your public key
6. Save