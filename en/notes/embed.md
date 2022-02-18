[Back to notes](/en/notes)
* * *
# How to user RT embed command
It is possible to make an embedding by doing the following.
```
rt!embed [url or webhook] "color code" title
content
```
If you set the part of `[url or webhook]` to `url`, you can create a URL where the embedded will appear when you send it.
If you set it to `webhook`, you can send an embedded with a webhook.  
In the case of `url`, it may not be reflected immediately. Let's wait. And there will be no newlines.  
In this case, you don't need to include the URL, but you won't be able to edit the message.  
The color code is embedded color, and please see [here] (https://rt-team.github.io/en/notes/color) for how to specify it.。  
In the case of web hooks, you can write the contents with markdown.  
So it is possible to write as follows.
```
rt!embed webhook "color code" title
description
## field
field description
## field
field description
## !Fields that don't line up sideways
Description of the field
## !Fields that don't line up sideways
Description of the field
### Fields in the field
※You can't make a deeper field.
```
Only one `#` can not be used,`## `or`## !`or` ### ` can be used.  
A field that does not line up is one in which the items in the field are never to the right of the previous field.  
The field can be on the right only in the web and PC versions of Discord, but on iOS, iPad OS, and Android, it is the same as the normal field.  
Also, in general markdown, you need to put two spaces when you start a new line, but you don't need to do this.

## Note
By default, the submitter of the embed will be the name of the executor and the icon will be the icon of the executor.  
This is because the embed is being sent using a webhook, so if you want the embed to be posted with the name and icon of RT, put `--rticon` before the title.  
That and putting `rt>embed` in the channel topic will automatically embed any message you send to that channel.  
You can also reply to something you have already created and run the command to edit it.

## Example
### Normal
```markdown
rt!embed url null welcome
First, let's check the rules with ## rules.
```
### Punishment history.
```markdown
rt!embed webhook red Punishment history
Kicked @tasuren.
## Reason.
Because he said something naughty.
```
### Rules.
```markdown
rt!embed webhook rule.
## !Rule 1
friendly
## !Rule #2
No NSFW stuff.
```