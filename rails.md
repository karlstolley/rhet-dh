## Ruby on Rails & Model-View-Controller (MVC)

I won’t go into a lengthy technical description of Ruby on Rails (just search the Web for it), but I will say that it is a Web development framework. Rails is installed on a computer via Ruby gems, a software package manager for the Ruby programming language, which Rails is written in.

Rails should be of interest to writer-programmers for many reasons, but my primary purpose in showcasing it here is that Rails can be installed, invoked, and developed using only writing. There is no file to download and unzip (like Drupal, WordPress, and other platforms-as-frameworks that are currently popular). Rails is installed by running a command on the command line (indicated throughout this chapter by use of the dollar-sign, `$`):

    $ gem install rails

But installing Rails does not directly create a Rails application. Rather, having Rails installed provides access to its library of different modules, including those for handling models, views, and controllers. Rails also provides a command-line program, conveniently called `rails`; and it is with the `rails` command that a project is brought to life from the magical text-based command-line interface (CLI). In this case, I am creating a new project called Magus, whose purpose will be to enable someone to input single lines of source code or command-line input, and keep notes as to the usefulness or significance of those lines. Basically, Magus will be a commonplace book for source-level writing:

    $ rails new magus

A bunch of output will fly by, leaving a directory of the application’s name, in this case, `magus`. Changing into the `magus` directory reveals that `rails` has created numerous new files and directories (identifiable below by lines ending in a slash, `/`), which can be listed via the CLI’s `ls` command on Unix-like systems:

    $ ls -lA1p
    .gitignore
    Gemfile
    Gemfile.lock
    README.rdoc
    Rakefile
    app/
    config/
    config.ru
    db/
    doc/
    lib/
    log/
    public/
    script/
    test/
    tmp/
    vendor/

At this point, another technology can be brought to bear both to aid in the development of the Web application, and also to help showcase the intellectual work of digital development of this nature: a content versioning system (CVS). Rails is configured out of the box (OOTB) to work with the distributed CVS Git (thus the `.gitignore` file that Rails generates, which will force Git to keep certain files out of the application’s repository).

Running `git init` from the command-line on a system that has Git installed prepares the repository, while running `git add .` stages all of the files for being written to the history of the project. The actual recording of history, a “commit” in Git parlance, is achieved in the short form via the `git commit` command, along with a message describing the contents of the commit, e.g.:

    $ git commit -m "Initial commit; OOTB Rails 3.2.11 application"

A bunch of output will fly by; running `git log` from the CLI will now reveal the information describing this initial commit:

    $ git log
    commit 09b803017e65c734354ce8ed24c06c55ae07ba43
    Author: XXX YYYY <xxx.yyyy@gmail.com>
    Date:   Wed Feb 6 13:27:48 2013 -0600

        Initial commit; OOTB Rails 3.2.11 application

This first commit, marking only the output created by Rails OOTB, will forever be identified by SHA-1 hash listed on the line beginning with the word `commit` in the CLI output. At any point, a writer may use the `git diff` command followed by this and any other commit’s SHA-1 hash and learn exactly which lines of code were the creation of the writer.

Rails is intended for sophisticated development, but done on the writer’s own computer. For this reason, Rails actually ships with a Web server called WEBrick, which can be started by running `rails server` from the CLI:

    $ rails server
    => Booting WEBrick
    => Rails 3.2.11 application starting in development on http://0.0.0.0:3000
    => Call with -d to detach
    => Ctrl-C to shutdown server
    [2013-02-06 13:33:48] INFO  WEBrick 1.3.1
    [2013-02-06 13:33:48] INFO  ruby 1.9.3 (2012-04-20) [x86_64-darwin12.0.0]
    [2013-02-06 13:33:48] INFO  WEBrick::HTTPServer#start: pid=12829 port=3000

With the server running, opening a Web browser to http://localhost:3000/ will show the default “Welcome aboard!” message indicating that Rails is operational, with a hyperlink provided to reveal the details of the writer’s development environment.

What this means is that by writing two simple phrases (`rails new magus` and `rails server`), a writer is able to create the skeletal outline of a Web application and launch a server to view the application exactly as it will be scene by the public Web once the app has been deployed.

Of course, what the `rails new` command builds is not much of an application at all. To move closer to becoming a Web application, a writer must do some more writing--issuing additional incantations on the CLI to describe the basic pieces of information that this Web application will be responsible for creating and maintaining.

Conveniently parallel to Covino’s generative magic, the first real writing of a Rails app makes use of the `rails generate` command. As the app is going to store single lines of code or CLI input, along with a note, I will create an object, which I’m calling Commonplace, that stores exactly those two things in the Magus app:

    $ rails generate scaffold Commonplace sourceline:string note:text


