logstash-logback-encoder
========================

This repository is intended to reference stored artifacts from
https://github.com/logstash/logstash-logback-encoder in Wikimedia's Gerrit
instance, via git-lfs.  This is useful for example to deploy such artifacts
via trebuchet by including this repository.

Not all dependency artifacts have been imported, if you require one of the
dependencies listed as optional, perform the following steps:

1. Make sure `git-lfs` has been initialized for this repository:
```
git lfs install
```
2. Copy the desired artifact into this repository, and add it to git, and commit:
```
cp /from/somewhere/else/myspecial-1.0.0.jar lib/
git add lib/myspecial-1.0.0.jar
git commit
```
3. Push the commit to Gerrit for review
```
git push origin HEAD:refs/for/master
```
