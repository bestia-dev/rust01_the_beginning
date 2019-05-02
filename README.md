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
1. Go to https://www.rust-lang.org and choose "GET STARTED".  
2. Find the RUSTUP-INI.EXE (6MB) Download it and run it.  
3. Windows Defender will warn you that the app is unrecognized. Choose "More info" and "Run anyway". Take your responsabilities.  
4. Read the text in the console and answer with default choices. They are ok for the first time install.  
5. It will download and install a number of tools and documentation. Be patient with the docs, they take a looong time. There is a big discussion in the Rust community to not install them by default and let the user choose them later. But now we have what we have.  
That's it. Rust is installed. Super simple.  

## The first project  
Press "window+s" (window is this strange key on the keyboard) it opens the start menu.  
Start typing "command prompt" it will suggest you exactly that and press Enter to run it.  
You should be inside your user folder. For me it is C:\Users\Luciano.  
I created a folder with the name all smallcaps "rustprojects" inside my user folder.  
In Windows file/folder names are not case sensitive, but in Linux they are. Be carefull.  
`mkdir rustprojects`  
`cd rustprojects`  
We will create a new rust project with this simple command  
`cargo new first_hello`  
`cd first_hello`  
You probably already know that you can type just `cd f` and then press the Tab key multiple times to get suggestions of subfolders name starting with f. If not, try it. It works great.  
  
Let build it and run it:  
`cargo run`  
Congratulations! You wrote your first working rust project.  
  
I am sure you want to try this again.  
Press the "arrow up". The command prompt will suggest the last typed command from history. In this moment it is `cargo run`. Run it by pressing Enter. This history is super usefull, because you will repeat the same commands a lot.  
This time the compilation is really fast, because there is nothing new to compile.  
## VSCode
Now you want to see and change the code. I choose the opensource editor VSCode.  
Download it and install it from here https://code.visualstudio.com/  
Run it and add a couple of extensions (Ctrl+Shift+X):
- Rust (rls)
- crates
- Better TOML
- Beautify  

Open your project with  
`File - Open Folder... - c:\users\Luciano\rustprojects\first_hello`  
Use your username here instead of mine.  
Simple Rust projects are basically just a folder. There is a convention of subfolders names and it works just that simple. You will find your code in the `src` subfolder in the file `main.rs`.  
Change the word `Hello` into `First Hello` and save it with `Ctrl+s`.  
You already know from before how to build and run it. Give it a try and show what you have learned.  

TODO:  
## Git

## WSL Windows subsystem for Linux
In the command prompt you can use %HOMEPATH% in windows is like ~ in Linux. It is your user folder. For me is C:\users\Luciano  
Windows can very often understand both \ and / as folder delimiters, but not always. In Linux there is only /. So it is smart to learn to user / everywhere where it works.  


