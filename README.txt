A bosh release for my toy echo app.

Expects the BOSH directory to have a Cloud Config with:
- A VM type "tiny".
- A network named "manual".

```
wget https://www.python.org/ftp/python/2.7.12/Python-2.7.12.tar.xz -O ~/Downloads/Python-2.7.12.tar.xz
bosh add blob ~/Downloads/Python-2.7.12.tar.xz python_2.7.12
```

```
bosh create release --force
bosh upload release
```
