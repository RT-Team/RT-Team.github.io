[Return to Notes home](/en/notes)
* * *
# How to see help
## The difference between the web version
There is no difference.
The order of the display and command help is a bit different, that's all.

## Main
### Arguments of the command.
This is where you put the information that the command needs after the command in the form of letters.  
As an example, suppose there is a command `rt!love` that can be used to say either "I love you!" or "I hate you!".  
If I just run `rt!love`, RT doesn't know whether to say "I love you!" or "I hate you!".  
If you put `love` or `hate` after `rt!love`, then RT can decide whether to say love or hate.  
This `love/hate` part is the command argument.
#### How to read the command arguments
```markdown
**argument name** : what characters to pass
Description of the arguments
```
This is used in RT.  
Here is an example of the arguments in the help file for the `purge` command.  
You can also view it on Discord by running `rt!help purge`.  
```markdown
This is a message batch command.  
The explanation of message deletion by reaction is at the bottom.

Parameters
----------
count : int
    The number of messages to delete.
target : member's mention or name, optional
    Specify the sender of the message to be deleted.  
    If not selected, the message will be deleted regardless of the sender.
```
The command notation is as follows.  
`rt!purge <count> <target:option>`.  
After that, you can see that the arguments to the RT command are, as the name implies, a description of the arguments to that command.

#### About arguments with newlines or spaces
If you want to include an argument with spaces, enclose it with `"`.  
Otherwise, the character following the space will be used as the next argument.  
For example, let's say you want to run a command to remove the role `member` when the role `danger mute` is added.  
You would then do this. `rt!linker link danger mute member on`.  
But it doesn't work as expected.
This is because two arguments are used in `danger mute`.  
So we have to use `rt!linker link "danger mute" member on`.  
However, if it is the last argument of the command (the next argument doesn't exist), you don't need to put it between `"`.

#### What is the true/false value of an argument?
In some cases, the right side of an argument has a boolean value.  
This can be either `on` or `off`.

### What is an alias?
You may occasionally see an alias in the help.
This is a very useful thing and you should know about it.  
Here is an example of a command to create a recruitment panel called `recruitment`.  
Now, this command `recruitment` is long and annoying to type.  
For those who find it annoying, RT developers have prepared an alias for the command.  
The alias for `recruitment` is as follows from help.
```markdown
# Aliases
recruit, rct
```
In this case, `recruitment` can also be executed as `rct`.  
RT commands often have Japanese aliases, so if you read the help carefully, you will be able to run the commands more easily.  
That's good to know, my friend!

### About multiple commands in one help file.
The `tts` command, for example, does this.  
This does not mean that there are multiple commands, but that there are subcommands of a group command.
### What is a group command?
For example, the text-to-speak command `tts` has a command to start speaking, `rt!tts join`, and a command to disconnect, `rt!tts leave`.  
There is also the `rt!tts dictionary` dictionary command.  
And under this `dictionary`, there are also `add/remove` commands for adding dictionaries.  
A group command is one that combines multiple commands of a function into a single command.  
A subcommand is each command in the group command, which is the `join` of `rt!tts join`.  
In the case of such a group command, all subcommands of the command are described in the help of the command.  
So it's not like there are multiple commands in one.

### About RT prefixes
A prefix is something that is written at the beginning of a command so that when the command is executed, it is known that it is a Bot command.  
The prefix of RT is `rt!`.  
Actually, there are other prefixes that can be used to call RT besides the `rt!`.  
They are as follows:

* rt!
* rt.
* りつ！
* りつ.

So, if the command you are trying to execute has a Japanese alias, you can make all the commands you execute Japanese.

## About slashes.
See [here](/en/notes/slash_table)