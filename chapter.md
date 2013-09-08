# MVC, Materiality, and the Magus: The Rhetoric of Source-Level Production

* **Abstract** Writing is more than a metaphor for the activity of programming. Being steeped in the digital medium’s materiality and its own kind of magic, programming provides unique rhetorical and symbolic affordances for digital humanists producing objects intended for  screens across an expanding range of devices. Model-view-controller (MVC) architecture and the development of sophisticated patterns and idioms within contemporary languages, such as Ruby and the Rails framework, provide a scaffold to initiate sustained encounters with programming.

* **Keywords** programming, digital materiality, symbolic action, Ruby on Rails

> “The greater the range and intenseness of the opportunities for the exercising of our symbolic prowess, the greater might be our delight in such modes of action.” Kenneth Burke, “Rhetoric and Poetics,” *Language as Symbolic Action* (1966, 297)

Let me open with the major premise of this chapter’s argument: programming is writing. I mean that literally, as I will illustrate with some limited examples from the Ruby on Rails framework in this chapter. Though I mean the phrase literally, “programming is writing” is frequently invoked as a metaphor, even among programmers. I agree with programmer Steve McConnell (2004) who dismisses writing as “the most primitive metaphor for software development.” However there are some key points in his dismissal that are unsound. Among McConnell’s observations on the metaphor’s shortcomings:

* “[writing] doesn’t require any formal planning, and you figure out what you want to say as you go”
* “writing is usually a one-person activity”
* “in writing, a high premium is placed on originality. In software construction, [originality] is often less effective than focusing on the reuse of design ideas, code, and test cases from previous artifacts”

An oversimplified conception of writing forms the basis of McConnell’s critique of the metaphor. True, writing may not require formal planning, but as even the introductory-writing student quickly discovers, that’s an unstudied and ineffective way to proceed. Playwrights, poets, and technical writers alike know that writing is collaborative, to some degree, always. And from citation practices to genre features, writers have a wide foundation of reusable material upon which originality is built, given a particular rhetorical occasion: to write is to engage in intelligent, ethical (i.e., non-plagiarized) reuse of previous artifacts. However, as I discuss later, richer encounters with originality that digital writers and humanists alike might otherwise experience are routinely preempted by careless reuse and outsourcing of source-level production.

To provide a glimpse into the experience of programming, I will present some of the activities involved in building a web application using Ruby on Rails (a full Rails app is available with additional commentary via this book’s companion website). There isn’t room in this chapter for a full technical description of Ruby on Rails, but it’s enough for now to note that Rails is an open-source web-application development framework written in the Ruby programming language.

Rails can be installed, invoked, and developed entirely through writing. There is no file to manually download and unzip (as with Drupal, WordPress, and other platforms-as-frameworks that are currently popular), and nothing to click on. Rails is installed by running a command on any system with a command line (indicated here by the dollar-sign, `$`) and a Ruby installation, as is the case for Mac OS X and many distributions of Linux:

    $ gem install rails

Installing Rails does not create a Rails application. Among other things detailed below, a Rails installation includes a command-line program, conveniently called `rails`; and it is with the `rails` command that a project is brought to life from the text-based command-line interface (CLI). All that is required is a name for the project, which in this example I’ve chosen BeSocial, an imaginary social networking application:

    $ rails new besocial

On the command line, a bunch of output will fill the CLI screen, indicating the creation of a number of files directories, as well as the installation of additional software packages that a basic Rails app depends on. Two lines written on the command line have built the foundations for a web application developed through written programming activity. Running `rails server` on the command line within the new `besocial` directory fires up a web server that enables this newborn app to be viewed in a web browser at `http://localhost:3000`. I will return to the app at toward the end of the chapter.

## Materiality

When I claim that “programming is writing,” I am talking about writing source code right alongside and in service to acts of communication, including visual and interaction design. Yet for over 30 years, point-and-click interfaces have mediated writing and other forms of digital communication and design. Despite the benefits of those interfaces, their mediation has also obscured much of the rich symbolic activity happening just beneath the apparent simplicity of something like an iPad’s touch screen. Digital materiality would appear to be only screen-deep.

Jay David Bolter’s simple 1991 observation seems all but forgotten today: “Even a graphics program does not draw: it writes.” Working at a time even before the introduction of Microsoft Windows 3.1 and the mouse and graphical-user-interface (GUI) model of interaction that that operating system would make ubiquitous in ways the original Macintosh could not, Bolter could confidently proclaim as literal what now appears metaphorical: “All computing is reading and writing. The computer is therefore a technology for all writers—scientists and engineers as well as scholars, novelists, and poets” (10).

Just as McConnell oversimplified the activity of writing, so too do non-programmers generally oversimplify the activity of programming. To speak of “programming” as a vague, monolithic abstraction is no different from speaking of “cooking” or even “writing.” Any sustained, personal encounter with the activity reveals the vast complexity behind its abstraction. Although I am fascinated by books such as *10 PRINT* (Montfort et al. 2013) and certain other intellectual efforts emerging from the field software studies, it is not uncommon to encounter conference presentations and scholarship—including *10 PRINT*’s focus on a single line of BASIC—that showcase truly ancient source code, divorced (as with most writing) from the lived activity of its creation. Historical treatment of source code is, of course, as important as any other history of writing and media. But it is important to note that historical examples of source code typically differ greatly from contemporary programming languages such as JavaScript, Python, or Ruby. The materiality of source code has evolved, and with it, the activity of programming.

It is no huge leap to reformulate Bolter’s observation as “All *programming* is reading and writing.” Of course, outside of small groups of researchers in the field of rhetoric and other areas in the digital humanities, the idea that “programming is writing,” and therefore counts as intellectual work, is far from accepted. It’s not possible to seek acceptance for something that hasn’t been widely practiced, argued, and made known.

Ramsay and Rockwell (2012) note that, for those digital humanists “who have turned to building, hacking, and coding as part of their normal research activity,” there is a looming question of “whether the manipulation of features, objects, and states of interest using the language of coding or programming...constitutes theorizing.” Although far from arriving at any actionable answer to that question, Ramsay and Rockwell articulate the challenge that faces anyone who would claim that programming is literally writing, and therefore a mode of inquiry and intellectual work: those who program and build are compelled “to present their own activities as capable of providing affordances as rich and provocative as that of writing.”

The key word there is “activities”: it is neither the created artifact experienced on screen nor even the source code behind it alone that expresses the affordances of programming as intellectual work. It is the activity of programming itself that builders, writers-as-programmers must demonstrate. This activity, I believe, will ultimately present itself as “theorizing” as Ramsay and Rockwell seem to hope. But the path to theorization may look different from simply demonstrating to others a “rich and provocative” set of affordances meant to *metaphorically* suggest that “programming is writing.”

An approach to theorizing programming activity, perhaps based in rhetoric’s roots as a practical art that embraces theory as well as techne and craft, must be be articulated in order to demonstrate that programming is a knowledge-generating, epistemological activity. Along those lines, Malcolm McCullough observes that

> As we overcome the residual notion that computing is for objective documentation only, we
> must cultivate expressive sensibilities. These may result in a digital aesthetic or
> poetics.... And in the end, chances are that appropriate artifacts and descriptions will engage
> us through rich and transparent tools, built on newfound densities of symbolic notation and
> personally experienced as a medium. (1996, 219)

Unfortunately, the development of a fully realized, nuanced digital rhetoric that would account for the intellectual work of programming (i.e., the dense symbolic notation that McCullough anticipates) appears to be arrested by literary modes of knowledge-making, such as Ramsay and Rockwell’s fixation on a literary type of theorization. The screen artifact fails to demonstrate the intellectual work of programming, perhaps because screen artifacts are subject to the analysis of media historians and critics, whose methods appear closely related to literary modes such as close reading. The emerging field of software studies likewise concerns itself with a similar literary reading of source code.

Complicating matters, the “personal experience” of a medium that McCullough calls for is preempted by the ossifying tradition of outsourcing what could otherwise be knowledge-making work in the digital humanities. Outsource programming activity to third-party programmers, WYSIWYG interfaces, or readymade software packages like WordPress and Drupal, and it becomes even more difficult to realize McCullough’s calls for something as lofty as a digital aesthetic or poetics rooted in the symbolic materiality of programming.

For those of us who program as a crucial part of our research agendas, then, our argument must proceed by demonstrating that programming *as an activity* is genuine, humanistic inquiry that resists denigration with regard to more established knowledge-making activities grounded in the manipulation and interpretation of symbols.

The need for that line of argument draws writers- and humanists-as-programmers in close company to the knowledge-making practices of art and design. In an obscure but important pamphlet published by the Royal College of Art, Christopher Frayling (1993/4) urges differentiating between three craft-/activity-oriented modes of inquiry: research *into* art and design; research *for* art and design; and research *through* art and design.

Rhetoric and writing, as a humanistic example, have no small body of work that researches *into* writing, often by studying writers and their contexts, such as introductory writing students in first-year composition or seasoned technical writers working in industry. The research conducted *for* writing often takes a pedagogical turn: this line of inquiry is aimed at making writing more teachable to students, rather than necessarily to improve the practice of writing itself.

But it is Frayling’s last prepositional category, research *through* writing and rhetoric—that is, as I am arguing, *through* programming as “personally experienced” symbolic activity—that remains an undervalued mode of knowledge-making.

## Magic & Programming

Programming is writing. Programming is symbolic, knowledge-making activity. To program, as to write, is to inquire and act in the realm of the symbolic. “Making language has long been regarded as, in some sense, magical; as a *spell*” writes William Covino in *Magic, Rhetoric, and Literacy*, adding “spelling, even in its ostensibly nonmagical sense, denotes the visible materialization of invisible thought” (1994, 5).

Decades before Steve Jobs introduced to the world the iPad and proclaimed it to be a magical device, Arthur C. Clarke had already articulated what has become known as Clarke’s Third Law: “Any sufficiently advanced technology is indistinguishable from magic.” It is no feat of imagination to see the magic inherent in 64-bit color depths, multitouch interfaces, retina displays, and other hardware-based wonders of screens introduced over the last decade.

But the magical incantation of the written word in one programming language or another is what  makes the symbolic activity of programming a particularly interesting problem for rhetoric and the digital humanities more broadly. Emerging production methods such as responsive web design (RWD; see Marcotte 2010) provide clear evidence that it is the written word, not a readymade interface, that opens up the affordances of newer screens, while still accommodating the old.

Reflecting on the scene from *The Matrix* in which Neo announces to Tank from inside the Construct that he needs “guns, lots of guns,” digital designer John Maeda describes “the sense of magic that occurs when Neo expresses his wish. The instantaneous rush of tremendous resources, as visualized in the simple special effect of this scene, epitomizes for me the experience of freedom when programming the invisible spaces of computer codes” (2004, 17).

While Maeda personally experiences “freedom,” of course, other people no doubt experience the fear inherent in contemplating the magical symbolic activity of programming. Fear that stems from closing ourselves off from personal experiences of the digital medium realized through programming. “Fear of magic has always been with us, in particular the fear of magic words...which claim to define or alter reality” (Covino 1994, 1). It’s no coincidence that *The Matrix* is set in a simulated/altered reality that is achieved purely by source code, which the viewer passes through in *The Matrix*’s opening title sequence.

In addition to the privileging of literary modes of inquiry that I noted above, there is also a problem within the humanities and its culturally-inherited mythos of programming as a mysterious and magical activity. That mythos is probably reinforced by the intercession of so many screens and interfaces that provide both a sanctioned visual kind of magic (the GUI) and tacit promises of protection from a disruptive, unpredictable textual kind of magic (programming).

Covino’s treatment accounts for precisely those two oppositional senses of magic: as “arresting magic,” programming would indeed by conjured only by a particular magus, the programmer, whose spells and incantations (realized in visual interfaces from word processors to smart phones) represent “the imposition of the powerful few upon the unquestioning many” (1994, 8). However, magic presents itself in another sense: “the practice of disrupting and critiquing articulate power: a (re)sorcery of spells for generating multiple perspectives.” Noting that “generative magic enters the world it questions,” Covino argues that generative magic is therefore “an amplification of the possibilities for action” (8).

How are digital humanists, such as digital writers, to discover the possibilities for action such as inquiry, if not through extended personal encounters with programming that “enters the world it questions”? Situated as I am in the study of digital rhetoric and design/development, this is the digital humanities that I envision and pursue: research *through* programming that creates knowledge that will push the digital humanities in general, and rhetoric more specifically, into ever more nuanced conversations with regard to the theory and practice of symbolic action made possible by programming.

## Model-View-Controller

Not only have the syntaxes of programming languages evolved, but so too have the paradigms and idiomatic forms within given languages. To conclude this chapter, I want to provide a brief overview of a specific software construction paradigm, model-view-controller (MVC) as implemented in the Ruby on Rails framework.

MVC is a software design pattern that abstracts and separates three essential components of any digital system controlled, importantly, by a graphical user interface. Originally designed at Xerox PARC by Trygve Reenskaug in the late 1970s, MVC was intended to “to bridge the gap between the human user’s mental model and the digital model that exists in the computer” (Reenskaug 2008). The View provides a visual interface to data described by the Model. The Controller exists to respond to actions occurring with in the View and makes requests to the Model.

## Bibliography

Bolter, Jay David. 1991. *Writing Space: The Computer, Hypertext, and the History of Writing*. Hillsdale, NJ: Lawrence Erlbaum Associates.

Burke, Kenneth. 1966. *Language as Symbolic Action: Essays on Life, Literature, and Method*. Berkeley, CA: University of California Press.

Covino, William A. 1994. *Magic, Rhetoric, and Literacy: An Eccentric History of the Composing Imagination*. Albany, NY: Statue University of New York Press.

Frayling, Christopher. 1993/4. “Reseach in Art and Design.” *Royal College of Art Research Papers* 1, no. 1.

Maeda, John. 2004. *Creative Code*. New York, NY: Thames and Hudson.

Marcotte, Ethan. 2010. “Responsive Web Design.” *A List Apart: For People Who Make Websites*, May 25. http://alistapart.com/article/responsive-web-design

McConnell, Steve. 2004. *Code Complete*. 2nd ed. Redmond, WA: Microsoft Press. Kindle edition.

McCullough, Malcolm. 1996. *Abstracting Craft: The Practiced Digital Hand*. Cambridge, MA: The MIT Press.

Montfort, Nick, Patsy Baudoin, John Bell, Ian Bogost Jeremy Douglass, Mark C. Marino, Michael Mateas Casey Reas, Mark Sample, and Noah Vawter. 2013. *10 PRINT CHR$(205.5+RND(1)); : GOTO 10*. Cambridge, MA: The MIT Press.

Ramsay, Stephen and Geoffrey Rockwell. 2012. “Developing Things: Notes toward an Epistemology of Building in the Digital Humanities,” in *Debates in the Digital Humanities*, edited by Matthew K. Gold. Minneapolis, MN: University of Minnesota Press. Kindle edition.

Reenskaug, Trygve M. H. 2008. “MVC: Xerox PARC 1978-78.” http://heim.ifi.uio.no/~trygver/themes/mvc/mvc-index.html

