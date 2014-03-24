Summary )
"sgit" is a tool that help programmers(especially system administrators) to manage single, that is to say, unprojected, files with git. For example, a little script, an bashrc, an vimrc, etc.

Installation )
If you have root permision of your system, just type './sgit install' to copy sgit script to /usr/bin. That's all.

Usage )
Type 'sgit filename' to track a file. Whenever you made a change on the tracked file, just use 'sgit ci filename' to commited. The git repo is at your $HOME/.sgit , so you can cd to the directory and use any git command you need. For convinience, sgit wrapped a bit of git command:
sgit ci filename (we metioned above)
sgit list (list the files managed by sgit)
sgit setremote (provide a friendly interactive interface to set git remote server for sgit repository, after set this, you can use 'sgit pull' and 'sgit push')
sgit pull (pull code from remote)
sgit push (push code from remote)

Background )
The idea of sgit is very simple: to make unprojected files being tracked by git, sgit create an git repository at $HOME/.sgit, then make an HARD LINK into it for the file you want to track. Then do a little wrap on git subcommand to bring some convinience. The script is easy to understand, for more information, just read it.

Have fun (-;

Bukn Zhang
zhcfreesea@gmail.com
