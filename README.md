# CentOS 7 yum repository

> Working CentOS 7 yum repository files to replace the .repo files in your /etc/yum.repos.d folder on your CentOS 7 server.

## Usage:
Navigate to the `/etc` folder:
```bash
cd /etc
```

</br>

Backup your current `yum.repos.d` folder first:
```bash
mv yum.repos.d yum.repos.d_old
```

</br>

Clone the new `yum.repos.d` folder to your system:
```bash
git clone https://github.com/tkne/centos-7-repo.git yum.repos.d
```

</br>

Clean the local cache:
```bash
yum clean all
```

</br>

Update the installed packages on your system:
```bash
yum update
```

</br>

> [!IMPORTANT]
> In case you have other external repositories installed as well, you'll need to edit each .repo dotfile and replace the settings manually.