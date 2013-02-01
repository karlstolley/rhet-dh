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

The key word there is “activities.” It is not simply the created artifact, or the source code behind it, providing the affordances of intellectual work. It is the activity of programming itself that builders, writers-as-programmers must present. It is what I will attempt to present in an artificial case over the remainder of this chapter.

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

But installing Rails does not actually create a Rails application. Rather, it provides access to its library of different modules, including those for handling models, views, and controllers. Rails also provides a command-line program, conveniently called `rails`; and it is with the `rails` command that a project is brought to life. In this case, I am creating a new project called `magus`:

    $ rails new magus

A bunch of output will fly by, leaving a directory of the application’s name, in this case, `magus`. Changing into the `magus` directory
----


Correcting one problem, especially through the ubiquitous WYSIWYG interface that outputs code on behalf of the writer, spirals into a game of Whack-a-Mole, introducing new problems whose solutions introduce still other problems. The same is true of throwing plugin upon plugin into Drupal and WordPress installations that stand as wholesale acts of reuse as invention. Download, unzip, upload, and run an install script.







For the magus, words transform reality, and facility with language makes multiple realities possible. (Covino 6)

Any sufficiently advanced technology is indistinguishable from magic. --Arthur C. Clarke



