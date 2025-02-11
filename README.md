# IBM i Notebooks

<img width="1313" alt="Screenshot 2022-03-05 at 11 27 00 AM" src="https://user-images.githubusercontent.com/3708366/156892015-bb9a935c-638d-4542-8b26-ebfedfbfbf10.png">

Adds an IBM i Notebook, which allows users to create notebooks to:

* run CL commands
* run commands in PASE (`shellscript`)
* execute SQL statements

**Depends on Code for IBM i.**

## What is the point of a Notebook?

> Notebooks are documents that contain a mix of rich Markdown, executable code snippets, and accompanying rich output. These are all separated into distinct cells and can be interleaved in any order.
>
> Notebooks are great storytelling devices, allowing you to interleave Markdown elements like images, math equations, and explanatory text with your code. Notebooks can be a perfect way to share and explain your ideas with coworkers or the public community.

*[Read more on the Visual Studio Code website.](https://code.visualstudio.com/blogs/2021/11/08/custom-notebooks)*

## How to use

1. Connect to an IBM i using Code for IBM i.
2. Create a file with the `.inb` extension
3. Open an `.inb` file
   * You can open `.inb` files in the IFS, **or**
   * You can make a source member with type `INB`,
   * You can open local `.inb` files,
   * You can also use the 'New Notebook' command to create a new local Notebook. Use F1/Ctrl+Shift+P and search 'new notebook'

## CL commands

When CL commands are executed, they will use the library list that is setup in Code for IBM i. If you have CL content assist enabled (as part of Code for IBM i), then you will be able to use utilise that when writing CL commands.

## SQL statements

SQL statements run in SQL mode (`*SQL`) and will always have a default library that matches the user's user profile name. Any unqualified objects will use the default library.
