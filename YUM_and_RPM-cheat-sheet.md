Yum and RPM cheat sheet
========

# Yum

## List all repository

```yum repolist```

## List all packages availables in a single repo

```yum --disablerepo="*" --enablerepo="google" list available```

## From which repo this package comes from

```yum info <package>```

## Search for package and show duplicates

```yum search --showduplicates jdk```

# RPM

## List all files of an installed package

```rpm -ql <intstalled-package>```

## List all files inside an rpm file

```rpm -qlp </local/package.rpm>```

## Find which rpm a file belong to

```rpm -qf </local/file>```

## Extract files from a RPM

```rpm2cpio <package.rpm> | cpio -idmv```

## Install an RPM in a different directory:

```rpm -ivh --prefix=</local/path< <package.rpm>```
 
