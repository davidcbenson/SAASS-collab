This page will give you some tools for note taking and accessing.
The most important thing you can do is use something that works for you.
Many people in the SAASS classes are digital natives&mdash;they have always had computers to help them in their lives&mdash;but may not know about these tools.
For others, those who are less comfortable with computers, using these tools can be an obstacle, not a help.
There is no wrong way to do this; don't try to force yourself to fit into a workflow you aren't comfortable with.

# Note Taking
In general, there are two ways to take notes: linear or non-linear.
Linear is a common way to take notes during a lecture or speech.
Linear can be useful when order matters.
Non-linear works well in situations where the order things arise may not be important.
Some people don't think linearly, either, and trying to force an order onto them is painful.

## Linear notes.

### Text Editors

One of the easiest ways to take linear notes is with a text editor.
Word is **not** a text editor; notepad  is.
The advantage of text editors include:
  * they can be read on any device, and don't normally need a special program
  * the files are subject to less security problems (no viruses)
  * they can be easily encrypted
  * small files
  * little temptation to futz with formatting while taking notes

Disadvantages are:
  * strictly linear
  * few formatting options
 
There are a number of great, free text editors out there, and if you don't have a preferred one, you should experiment with one, even if you won't use them to take notes.
Some of the more common, or easy to use text editors include:

  * [Atom](https://atom.io/) 
  * [Notepad++](https://notepad-plus-plus.org/)
  * [Vim](http://www.vim.org/)
 
If you are new to text editors, or want something fairly easy and full featured (or you want Prof. Benson to be able to help you) you should go with Atom.
Vim is great, but has a steep learning curve, which is worth it for people who will do a lot text editing, but not so much for others.

##### Markdown

Although text files themselves do not have formatting, there is something called "Markdown" that can both add formatting or substitute for it in text files.
Github, the host of this repo, uses markdown a lot, and [has a great tutorial](https://guides.github.com/features/mastering-markdown/).
This page, and others like it are also written in markdown, and you can see the markdown if you look around.
You can use tools for markdown elsewhere such as [Markdown Here](http://markdown-here.com/), too.
Of course, the nice thing about Markdown is that it is easily legible, even when not converted, and can be used and read in text files alone.

### Word

Word is not a text editor.
It has a proprietary file format (.doc, or .docx) which requires decoding to be read.
That said, it can be used as a text editor, just save files as .txt files, and you are good to go.

Word has some advantages that lend itself to note taking, including:
  * familiar to almost everyone
  * Very common
  * More formatting options
  * Some non-linearity is possible
  * Review is popular for collaboration
 
 The disadvantages include:
   * Poor security (Macro virus, etc.)
   * Formatting doesn't transfer easily outside the MS ecosystem, and can go awry easily
   * Version control is hard
   * Files are much larger than necessary



Word, in many ways, is sort of the "good enough" of note takers.
It is good at most things but not great at anything.
Use Word if it works for you, but don't feel like it is the only option, especially if you need something that is great at something.

### Onenote

This is a Microsoft product, so it will be comfortable to most people.
It is made for note taking, and free versions are available for the iPhone and Android.

As a specifically note taking product it has a lot of advantages for not taking, including:
  * made to work like notebooks, so works very well with linear or traditional note takers
  * Support for drawings, tables etc.
  * Non-linear options exist
  * Lots of add-ons
  * Corporate support

Negatives exist too:
  * Huge files
  * The same security challenges as with Word
  * You have to have a version of Onenote to read any of the files

On balance, this is a very good note taker, which works for a lot of people, but which may not be for everyone.

### Evernote

I have never used it, so I can't tell you how it works.
Some people love it though.
It does most of the same things that Onenote does.
The differences between the two are describe as "Onenote is made to work like a notebook, whereas Evernote is made to work like a filing cabinet."

# Getting Information Out

If you use Onenote or Evernote, the organization is part of the program. 
Otherwise, you need to think about organization for your files and notes, so you can find what you need.
Microsoft offers a [tutorial for Onenote][onenote] and there is a tutorial for Evernote, [on their website][evernote], too.
Those tutorials will get you started.

## Tagging

In Word documents, it is possible to tag files with keywords, and search or filter by those keywords.
This is *incredibly* helpful when trying to find content, as it allows more than one way to find information.
You can also use a pseudo-tag, by including keywords at the beginning of files, and searching for them.
There are many tutorials online how to do this, [including this one][tagging].

## Searching
For the most part, this is what many people do, and it isn't a bad option.
The search function in any of the operating systems will usually find a file, so long as you have the correct box "Search inside files" checked.
Searching works much more quickly with text files, and if it indexes the files, so you will want to save your files in one of the directories that your search indexes.
There are number of search programs, and some may work better for your search patterns or needs than others.
If you find the default search on your OS doesn't work for you, consider trying one of the 3rd party options.

## File Folders and Soft/Hard Links

One of the oldest ways to categories files is in folders, and it is the most intuitive to people who are used to file cabinets. 
Unfortunately, if you have a folder named "Cyber" and "China" and you have a file which is about cyber in China, you may be forced to make a choice.
That is where links come in.

Soft links are essentially the same as shortcuts on windows, and for the purposes of finding files you can actually substitute shortcuts for soft-links.
The link just redirects you to a different file location.
The advantage is that they are easy to do both in command line, and in the GUI.
You can't process or search soft links though.

[Hard links point the computer to the same file](https://msdn.microsoft.com/en-us/library/windows/desktop/aa365006(v=vs.85).aspx), but from two different locations.
The names can even be different in different directories, but the file will open the same, because it **is the same file.**
The advantage is you can treat a hard link exactly like you treat a file, including searching and so on.
The disadvantages are it is complicated and you can accidentally create circular links which will be very bad for your computer.
Furthermore, if you delete a softlink, only the link, not the file goes away, but if you delete a hard link, "both" files disappear, so you have to be careful.
I love hard links, but highly recommend that you only link to files not directories, to make sure this problem doesn't arise, at least until you are more familiar with them.


## Databases

Using a database is probably the most reliable, but with the most maintenance and upfront costs.
The database can be a traditional database like SQLite, MySQL or MS Access.
Alternatively, you can you a citation managing database like Zotero or JabRef to manage your notes.

Setting up a database, or using a highly customizable citation manager allows a lot of variation, which means you can make the database fit your note taking style.
"Off the Shelf" systems are often less customizable, and therefore you have to change what you do, but usually the system works by itself.

Many of your notes will be on books or articles anyway, so it makes sense to keep all notes in the citation manager.
However, citation managers are not made for most analytical tools, so if you plan on using data management software for any kind of analysis a specialized database may be necessary.

If you want to try your hand at creating a database, you are most likely best starting with [MS Access][access] which has a great tutorial online from Microsoft, and most people already have installed on their computer.
To get the most out of the database, you probably want to learn [a little SQL][sql] at least, though.



  [onenote]: https://support.office.com/en-us/article/OneNote-2016-training-51d1d95b-bdf4-48df-acad-a3331dec8f97
  [evernote]: https://help.evernote.com/hc/en-us/categories/10681-Tips-Tutorials
  [tagging]: https://wordribbon.tips.net/T005952_Using_Tags_with_Document_Files.html
  [access]: https://support.office.com/en-us/article/Access-2013-videos-and-tutorials-a4bd10ea-d5f4-40c5-8b37-d254561f8bce
  [sql]: https://www.w3schools.com/SQL/deFault.asp
