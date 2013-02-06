# MVC, Materiality, and the Magus: The Rhetoric of Source-Level Production

“The greater the range and intenseness of the opportunities for the exercising of our symbolic prowess, the greater might be our delight in such modes of action.” Kenneth Burke, “Rhetoric and Poetics,” *Language as Symbolic Action*, p. 297

Let me open with the major premise of my argument: programming is writing. I mean that literally. Yes, “programming is writing” is not infrequently invoked in a metaphorical sense. And I agree with programmer Steve McConnell who dismisses writing as “the most primitive metaphor for software development.” Among McConnell’s observations on the metaphor’s shortcomings:

  * “[writing] doesn’t require any formal planning, and you figure out what you want to say as you
    go”
  * “writing is usually a one-person activity”
  * “in writing, a high premium is placed on originality. In software construction, [originality] is
    often less effective than focusing on the reuse of design ideas, code, and test cases from
    previous artifacts”
  * “when you finish writing a letter, you stuff it into an envelope and mail it. You can’t change
    it anymore”

Rhetoricians should immediately recognize the oversimplified conception of writing at the heart of McConnell’s critique. Writing may not require formal planning, but as even the introductory-writing student quickly discovers, that’s an unstudied and ineffective way to proceed. We know that writing is collaborative, on some level, always. And from citation practices to genre features, writers have a wide foundation of reusable material upon which “originality” is built. To write is to engage in intelligent, ethical (i.e., non-plagiarized) reuse of “previous artifacts.”

Granted, in certain forms of writing on certain occasions, change becomes impossible, or at least very difficult, in the way McConnell suggests. But even digital writing typically fares no better when it comes to revision and ongoing change. As I have argued elsewhere, one-off digital invention--as in the first (and typically, only) stab at even a basic web page--will have to suffice in the digital rhetorical act. There is simply too much risk involved in revision when digital production occurs apart from source code. When I declare that “programming is writing,” I am talking about writing source code right alongside or in service to natural languages. More than 30 years of visual interfaces interceding on behalf of writers and language (computer and natural) have arguably almost fully obscured the critical symbolic activity happening just beneath even the touch-screen on an iPad.

The remaining symbolic activity that hasn’t been obscured is perceived to be simply beyond our symbolic abilities. What could be more preposterous than writers programming? “Making language has long been regarded as, in some sense, magical; as a *spell*” writes William Covino in *Magic, Rhetoric, and Literacy*, adding “spelling, even in its ostensibly nonmagical sense, denotes the visible materialization of invisible thought” (Covino, 5). Visual interfaces, particularly those for digital production and expression, are readymade materializations of invisible thoughts of programmers. We are compelled by arresting interfaces to compose through other people’s interfaces, other people’s text boxes.

Of course, outside of small groups of individuals in the field of rhetoric, particularly within Computers and Writing, the idea that “programming is writing,” or even that programming counts as intellectual work, is far from accepted. So it is within the broader pursuit of digital humanities. Ramsay and Rockwell note that, for those “who have turned to building, hacking, and coding as part of their normal research activity,” there is a looming question of “whether the manipulation of features, objects, and states of interest using the language of coding or programming...constitutes theorizing” within the digital humanities. Although far from arriving at any actionable answer to that question, Ramsay and Rockwell articulate the challenge that faces anyone who would claim that programming is literally writing: those who program and build are the only people “to present their own activities as capable of providing affordances as rich and provocative as that of writing.”

The key word there is “activities.” It is not simply the created artifact, or the source code behind it, providing the affordances of intellectual work. It is the activity of programming itself that builders, writers-as-programmers must present. It is what I will attempt to present in an artificial case of writing a simple Web application over the remainder of this chapter.

## Magic & Programming

Decades before Steve Jobs pronounced the iPad to be a magical device, Arthur C. Clarke had already articulated what has become known as Clarke’s Third Law: “Any sufficiently advanced technology is indistinguishable from magic.” It is no feat of imagination to see the magic inherent in multitouch interfaces, retina displays, ubiquitous high-speed internet connectivity, and other hardware-based wonders introduced over the last decade.

But the magical incantation of the written word in one programming language or another is what makes the magic. Jay David Bolter’s simple 1991 observation seems all but forgotten today: “Even a graphics program does not draw: it writes.” Writing at a time before the introduction of Microsoft Windows 3.1 and the mouse-and-GUI model of interaction that that operating system would make ubiquitous, Bolter could confidently proclaim what is less obvious today: “All computing is reading and writing. The computer is therefore a technology for all writers--scientists and engineers as well as scholars, novelists, and poets” (10).

Recalling the scene from *The Matrix* where Neo announces to Tank from inside the Construct that he needs “Guns. Lots of guns,” digital designer John Maeda describes “the sense of magic that occurs when Neo expresses his wish. The instantaneous rush of tremendous resources, as visualized in the simple special effect of this scene, epitomizes for me the experience of freedom when programming the invisible spaces of computer codes” (*Creative Code*, 17).

Where Maeda experiences “freedom,” of course, other people no doubt experience the fear inherent in contemplating the magical symbolic activity of programming. “Fear of magic has always been with us, in particular the fear of magic words...which claim to define or alter reality” (Covino 1). Yet “Even in our nonmagical world, magic remains a conceptual construct for appraising the powers of language, and while magic is understood by some as a liberatory alternative to established rationalism, the prospect of a magical epistemology is a fearful one even for those who endorse literacy as a disruptive force” (5). Programming presents itself as magic to the uninitiated. I have witnessed that even just the prospect of programming can arrest into silent hostility rhetoricians and writers who otherwise “endorse literacy as a disruptive force” and who ostensibly delight in an ever greater “range and intenseness” of symbolic activity (as Burke suggests in the epigraph to this chapter).

But magic is not simply magic. In what Covino describes as “arresting magic,” programming would indeed by conjured only by a particular magus, the programmer, whose spells and incantations (from word processors to smart phones) represent “the imposition of the powerful few upon the unquestioning many” (8). However, magic presents itself in another sense: “the practice of disrupting and critiquing articulate power: a (re)sorcery of spells for generating multiple perspectives.” Noting that “generative magic enters the world it questions,” however, Covino argues that generative magic is “an amplification of the possibilities for action.”

A fully realized, nuanced digital rhetoric has been arrested by the WYSIWYG interface. In fact, I don’t think a rhetoric of programming is possible to articulate at the moment; there are simply not enough of us who program. And those of us who do program have yet to argue that the artful manipulation of symbols that constitutes programming should not be distinguished from or denigrated with regard to any other activity traditionally considered “writing.”

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


