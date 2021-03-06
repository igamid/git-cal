git-cal
=======

### Description
![screenshot with black theme](https://raw.github.com/k4rthik/git-cal/master/screenshots/img1.png) 
![screenshot with white theme](https://raw.github.com/k4rthik/git-cal/master/screenshots/img2.png)
on your terminal

* git-cal is a simple script to view commits calendar (similar to github contributions calendar) on command line
* Each block in the graph corresponds to a day and is shaded with one
  of the 5 possible colors, each representing relative number of commits on that day.
* Opt out from ANSI colors and use few ASCII characters to denote the same.

### Install

Just drop the script anywhere in $PATH or
- with root access:
```
perl Makefile.PL
make
sudo make install
```

- without root access:
```
perl Makefile.PL PREFIX=~/.local
make
make install
```

### TODO
- Fix issue with --author parameter, this might mean finding an alternative to Getopt::Long.
- Support --github=<username> parameter to pull activity calendar using github api (if possible/authenticated, get private repos too)
- Support more statistics like commits per month/week etc
- May be add a small conf file to customize colors/characters.
- Make the code pretty and modular so that will be easy to extend.

