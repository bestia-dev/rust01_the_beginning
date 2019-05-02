Things are changing fast. This is the situation on 2019-05-02. Luciano Bestia  
# rust01_the_beginning  
The first project in Rust. How to install the toolchain and have a first result in 5 minutes.  
There is almost always a lot of different ways to achieve some result. I will describe only one option - for simplicity.  
The learning process is easier if it is simple. But the reality is always much much more complicated then that.  
Knowledge must come in small drops to absorb it. If it is pouring it just confuses the curious mind.  
The "book" https://doc.rust-lang.org/1.0.0/book/ is a great learning tool. The first chapters are really easy and practical and very well written. Use it.   
## Windows  
I used Windows most of my long programmers life (33 years). It is still the number one desktop OS.  
So for developing desktop apps is a good start to have the developer environment inside Windows.  
1. Go to https://www.rust-lang.org and choose `GET STARTED`.  
2. Find the `RUSTUP-INI.EXE` (6MB) Download it and run it.  
3. Windows Defender will warn you that the app is unrecognized. Choose `More info` and `Run anyway`. Take your responsabilities!  
4. Read the text in the console and answer with default choices. They are ok for the first time install.  
5. It will download and install a number of tools and documentation. Be patient with the docs, they take a looong time. There is a big discussion in the Rust community to not install them by default and let the user choose them later. But now we have what we have.  
That's it. Rust is installed. Super simple.  

## The first project  
Press `window + s` (`window` is this strange key on the keyboard in the first row near `ctrl` and `alt`) it opens the start menu.  
Start typing `command prompt` it will suggest you exactly that and press Enter to run it.  
You should be inside your user folder. For me it is `C:\Users\Luciano`.  
I created a folder with the name all smallcaps `/rustprojects` inside my user folder.  
In Windows file/folder names are not case sensitive, but in Linux they are very sensitive. Be carefull.  
`mkdir rustprojects`  
`cd rustprojects`  
We will create a new rust project with this simple command  
`cargo new first_hello`  
`cd first_hello`  
You probably already know that you can type just `cd f` and then press the Tab key multiple times to get suggestions of subfolders name starting with `f`.  
If not, try it. It works great.  
  
For most of the commands it is really important in what folder you run them. Now you should be inside the `c:\users\Luciano\rustprojects\first_hello` folder (with your username and not mine).  
Let build the project and run it:  
`cargo run`  
Congratulations! You wrote your first working rust project.  
  
I am sure you want to try this again one more time.  
Press the `arrow up`. The command prompt will suggest the last typed command from history. In this moment it is `cargo run`. Run it by pressing Enter.  
This history stuff is super useful, because you will repeat the same commands a lot.  
This time the compilation is really fast, because there is nothing new to compile.  
## VSCode
Now you want to see and change the code. I choose the opensource editor VSCode.  
Download it and install it from here https://code.visualstudio.com/  
Run it and add a vscode extensions for rust `Ctrl + Shift + X`:
- Rust (rls)
  
Open your project with  
`File - Open Folder... - c:\users\Luciano\rustprojects\first_hello`  
Use your username here instead of mine.  
Simple Rust projects are basically just a folder. There is a convention of subfolders names and it works just that simple. You will find your code in the `src` subfolder in the file `main.rs`.  
Change the word `Hello` into `First Hello` and save it with `Ctrl + s`.  
You already know from before how to build and run it. Give it a try and show what you have learned.  
## Git
Git is a great tool and you should use it for code versioning. Use it often and group the changes so that is easy to understand what a commit really changes.  
VSCode it totally prepared for it. I am not sure if you need to install it manually or VSCode makes all in its installation. You will quickly find out.  
The third icon on the left or `Ctrl + Shift + g` opens a simple list: what has changed. You write a `Message` and press `Ctrl + Enter` to commit.  
If you want to see the changes you select a filename. The changes will show on the right.  
You can also use it to push or sync the changes on GitHub and much more. Then there is a specific `.gitignore` file for rust source code. This is advanced stuff. You will learn it step by step.  

TODO:  
## WSL Windows subsystem for Linux
In the command prompt you can use %HOMEPATH% in windows is like ~ in Linux. It is your user folder. For me is C:\users\Luciano  
Windows can very often understand both \ and / as folder delimiters, but not always. In Linux there is only /. So it is smart to learn to user / everywhere where it works.  


