# Adding perma alias directly from terminal
yes its a bit useles u could just go on ur bash file (~/.zshrc or ~/.bashrc idk what ur using) and add it manualy
# but here's how to do it
here's what u need to do:
1. open ur terminal (not gonna tell u how, i think u know how to)
2. open ur terminal config file(~/.bashrc or idk search on google where it is) with ur fav text editor, u can do it with vsc using `code (path)`
3. go on ur last line and write this lil piece of code: 
```	
addpermalias() {
	echo "alias $1=\"$2\"" >> {ur config file (es: ~/.bashrc) w/out the brkt}
	source ~/.zshrc
}
```
4. change the part inside the bracket { }
5. save the changes (on vsc is ctrl+s idk on your editor)
6. have fun (yeee!)
# usage
simply close and re open ur terminal
and use it like this
`addpermalias namealias "associated command"`
# code analysis (sort of)
what the code does is really simple, whenever u use the command addpermalias adds a line to ur selected file, the new line will be formatted like this:
`alias alias="the thing"` 
the source part reload the config file, so u can use the command immediately 

ty for readin all dis, feel free to improve the code, this is my first serious repo on github so yk. byeee
