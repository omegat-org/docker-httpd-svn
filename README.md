# Unauthenticated Apache httpd with Subversion

This image provides Apache configured for use as a Subversion server *with no
authentication*. It is
[erikwramner/httpd-svn](https://hub.docker.com/r/erikwramner/httpd-svn) but with
authentication disabled.

*This image is for testing use only*

## Usage

To quickly get a Subversion server up and running with a test repository and a
single user, run:

```
docker run --rm -p 1234:80 -e SVN_REPO_NAME=test omegatorg/httpd-svn
```

That creates a Subversion repository named "test" and exposes it *with no
authentication* on port 1234.  The repository can be accessed at
http://localhost:1234/svn/test.

For any other uses, please use
[erikwramner/httpd-svn](https://hub.docker.com/r/erikwramner/httpd-svn) instead.
