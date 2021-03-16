# Learning Vim Editor

#### References
><a>http://yannesposito.com/Scratch/en/blog/Learn-Vim-Progressively/</a>

## 1. 1st Level - Survive

In a standard editor, typing on the keyboard is enough to write something amd see on the screen. Not this time! Vim starts on Normal mode. To go to ***Insert*** mode press i on the keyboard.

You should feel a bit better. You can type letters just like in a standard editor. To get back to ***Normal mode*** just press **ESC** key.

You now know how to switch between ***Insert*** and ***Normal*** mode.
Here are the commands you need to survive in Normal mode.

	- i →  insert mode. Type ESC to return to Normal mode.
	- x → Delete the character under the cursor
	- :wq → Save and Quit (:w save,, :q quit)
	- dd → Delete (and copy) the current line
	- p → Paste

Recommended:

	hjkl (highly recommended but not mandatory) → basic cursor move (←↓↑→). Hint: j looks like a down arrow.:help <command> → Show help about <command>. You can use :help without a <command> to get general help.

Only 5 commands. That's all you need to get started. Once these commands start to become natural (maybe after a day or so), you should move on to level 2.

>But first, just a little remark about Normal mode. In standard editors, to copy you have to use Ctrl key (Ctrl+C generally). In fact, when you press Ctrl, it is as if all of your keys change meaning. Using Vim in Normal mode is a bit like having the editor automatically press Ctrl key for you.

## 2. 2nd Level - Feel comfortable

You know the commands required for survival. It's time to learn a few more commands. Here are a number of suggestions.

### Insert mode variations:

	a → insert after the cursor
	o → insert a new line after the current one
	O → insert a new line before the current one
	cw → replace from cursor to the end of the word

### Basic moves:

	0 → go to the first column
	^ → go to the first non-blank character of the line
	$ → go to the end of the line
	g_ → go to the last non-blank character of the line
	/pattern → search for a pattern
	
### Copy/Paste
	P → paste before, remember p is paste after the current  position 
	yy → copy the current the line, easier but equivalent to ddP

### Undo/Redo
	u → undo
	<C-r> → redo

### Load/Save/Quit/Change File (Buffer)
	:e <path/to/file> → open
	:w → save
	:saveas <path/to/file> → save to <path/to/file>
	:x, ZZ or :wq → save and quit (:x only save if necessary)
	:q! → quit without saving, also :qa! to quit even if there are modified buffers
	:bn (resp. :bp) → show next (resp. previous) file (buffer)

Take time to learn all of these commands. Once done, you should be able do everything you were able to do in other editors. You may still feel unconfortable, but hold on to the next level and you will see why Vim is awesome.