microsite
=========

This is an attempt to provide a command-line mechanism for cloning a
repo. 

This is purely experimental at present.  Our goal is to create the
fastest possible way to create a personal site.

To use, clone this repo onto a computer that has bash.

Put your github password or access token into an environment variable
call GITHUB_PASSWORD.  Do NOT put this in the repo, to avoid the
danger of accidentally commiting it.

The run the bash script with 7 arguments:
1. The name of the new repo you wish to create.
2. A personal name
3. Your github account name under which you want to create the new
   repo.
4. Your github password (I prefer to use $GITHUB_PASSWORD)
5. The URL to the site you intend to clone.
6.  The "organization" under which you wish the repo to be created.
7. The name of the repo you are cloning from (this is duplication that
   someone could improve).

> 
> ./create_gh_site.bash siteclonetest1 Rob robertlread
> $GITHUB_PASSWORD https://github.com/18F/microsite-template1.git 18F
> microsite-template1

If the site, such as
https://github.com/MyInternetWebsite/microsite-template0 which is
meant to a template, contains the token:

> 663c8bbc10b66148ed44763d59a2ee4e

It will be replaced with the personal name given as the second argument.

# Rationale

This code provides a programmatic way to generate new repos.  For
example, you could use it to create 10 repos for a class teaching
people how to use github.

"With great power comes great responsibility." -- Spiderman

Be considerate of github and their users.

