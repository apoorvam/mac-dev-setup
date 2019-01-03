# Sublime Text

[Sublime Text](http://www.sublimetext.com/) is a sophisticated text editor for code, markup and prose. It has unlimited evaluation period, but if you wish to use the editor without any popups that come very often asking you to purchase, you can purchase it.

## Installation

You can download the installer [here], drag and drop it to Applications folder. 

## Launch from CLI

To launch Sublime Text from command line, create a symlink to its binary using below command:

```
ln -s "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl
```

Make sure `/usr/local/bin/` is already in your `PATH` variable. Now, you can use Sublime text to open a folder as `subl myProject` or a single file as `subl hello.go` directly from command line.