# MVC, Materiality, and the Magus: The Rhetoric of Source-Level Production

* **Abstract** Writing is more than a metaphor for the activity of programming. Being steeped in the digital medium’s materiality and its own kind of magic, programming provides unique rhetorical and symbolic affordances for digital humanists producing objects intended for  screens across an expanding range of devices. Model-view-controller (MVC) architecture and the development of sophisticated patterns and idioms within contemporary languages, such as Ruby and the Rails framework, provide a scaffold to initiate sustained encounters with source-level production.

* **Keywords** programming, digital materiality, symbolic action, Ruby on Rails

> “The greater the range and intenseness of the opportunities for the exercising of our symbolic prowess, the greater might be our delight in such modes of action.” Kenneth Burke, “Rhetoric and Poetics,” *Language as Symbolic Action* (1966, 297)

Let me open with the major premise of this chapter’s argument: programming is writing. I mean that literally, as I will illustrate with some limited examples from the Ruby on Rails framework in this chapter. Though I mean the phrase literally, “programming is writing” is frequently invoked as a metaphor, even among programmers. I agree with programmer Steve McConnell (2004) who dismisses writing as “the most primitive metaphor for software development.” However, there are some key points in his dismissal that are unsound. Among McConnell’s observations on the metaphor’s shortcomings:

* “[writing] doesn’t require any formal planning, and you figure out what you want to say as you go”
* “writing is usually a one-person activity”
* “in writing, a high premium is placed on originality. In software construction, [originality] is often less effective than focusing on the reuse of design ideas, code, and test cases from previous artifacts”

An oversimplified conception of writing forms the basis of McConnell’s critique of the metaphor. True, writing may not require formal planning, but as even the introductory-writing student quickly discovers, that’s an unstudied and ineffective way to proceed. Playwrights, poets, and technical writers alike know that writing is collaborative, to some degree, always. And from citation practices to genre features, writers have a wide foundation of reusable material upon which originality is built, given a particular rhetorical occasion: to write is to engage in intelligent, ethical (i.e., non-plagiarized) reuse of previous artifacts. However, as I discuss later, richer encounters with originality that digital writers and humanists alike might otherwise experience are routinely preempted by careless reuse and outsourcing of source-level production.

To provide a glimpse into the experience of programming, I will present some of the activities involved in building a web application using Ruby on Rails (a full Rails app is available with additional commentary via this book’s companion website). There isn’t room in this chapter for a full technical description of Ruby on Rails, but it’s enough for now to note that Rails is an open-source web-application development framework written in the Ruby programming language.

Rails can be installed, invoked, and developed entirely through writing. There is no file to manually download and unzip (as with Drupal, WordPress, and other platforms-as-frameworks that are currently popular) and nothing to click on. Rails is installed by running a command on any system with a command-line interface (CLI; indicated here by the dollar-sign, `$`) and a Ruby installation, as is the case for Mac OS X and many distributions of Linux:

    $ gem install rails

Installing Rails does not create a Rails application. Among other things detailed below, a Rails installation includes a command-line program, conveniently called `rails`; and it is with the `rails` command that a project is brought into existence. All that Rails requires is a name for the project, which in this example I’ve chosen BeSocial, an imaginary social networking application:

    $ rails new besocial

Running that command fills the CLI screen with dozens of lines of output indicating the creation of a number of files and directories, as well as the installation of additional Ruby software packages, called Gems, that a basic Rails app depends on. Two lines written on the command line have built the foundations for a web application developed through written programming activity. Running `rails server`from within the new `besocial` directory, which Rails created, starts a web server for the app. Although not much to look at yet, it can be viewed in a web browser at `http://localhost:3000/`. I will return to the construction of the app toward the end of the chapter.

## Materiality

When I claim that “programming is writing,” I am talking about writing source code right alongside and in service to acts of communication, including visual and interaction design. Yet for over 30 years, point-and-click interfaces have mediated writing and other forms of digital communication and design. Despite the benefits of those interfaces, their mediation has also obscured much of the rich symbolic activity happening just beneath the apparent simplicity of something like an iPad’s touch screen. Digital materiality would appear to be only screen-deep.

Jay David Bolter’s simple 1991 observation seems striking today: “Even a graphics program does not draw: it writes.” Working at a time even before the introduction of Microsoft Windows 3.1 and the mouse and graphical-user-interface (GUI) model of interaction that that operating system would make ubiquitous in ways the original Macintosh could not, Bolter could confidently proclaim as literal what now appears metaphorical: “All computing is reading and writing. The computer is therefore a technology for all writers—scientists and engineers as well as scholars, novelists, and poets” (10).

Just as McConnell oversimplified the activity of writing, so too do non-programmers generally oversimplify the activity of programming. To speak of “programming” as a vague, monolithic abstraction is no different from speaking of “cooking” or even “writing.” Any sustained, personal encounter with the activity reveals the vast complexity behind its abstraction. Although I am fascinated by books such as *10 PRINT* (Montfort et al. 2013) and certain other intellectual efforts emerging from the field software studies, it is not uncommon to encounter conference presentations and scholarship—including *10 PRINT*’s focus on a single line of BASIC—that showcase truly ancient source code, divorced (as with most writing) from the lived activity of its creation. Historical treatment of source code is, of course, as important as any other history of writing and media. But it is important to note that historical examples of source code typically differ greatly from contemporary programming languages such as JavaScript, Python, or Ruby. The materiality of source code has evolved, and with it, the activity of programming.

It is no huge leap to reformulate Bolter’s observation as “All *programming* is reading and writing.” Of course, outside of small groups of researchers in the field of rhetoric and other areas in the digital humanities, the idea is far from accepted that “programming is writing” and therefore counts as intellectual work. It’s difficult to seek acceptance for something that hasn’t been widely practiced, argued, and made known.

Ramsay and Rockwell (2012) note that, for those digital humanists “who have turned to building, hacking, and coding as part of their normal research activity,” there is a looming question of “whether the manipulation of features, objects, and states of interest using the language of coding or programming...constitutes theorizing.” Although far from arriving at any actionable answer to that question, Ramsay and Rockwell articulate the challenge that faces anyone who would claim that programming is literally writing, and therefore a mode of inquiry and intellectual work: those who program and build are compelled “to present their own activities as capable of providing affordances as rich and provocative as that of writing.”

The key word there is “activities”: it is neither the created artifact experienced on screen nor even the source code behind it alone that expresses the affordances of programming as intellectual work. It is the activity of programming itself that builders, writers-as-programmers must demonstrate. This activity, I believe, will ultimately present itself as “theorizing” as Ramsay and Rockwell seem to hope. But the path to theorization may look different from simply demonstrating to others a “rich and provocative” set of affordances meant to *metaphorically* suggest that “programming is writing.”

An approach to theorizing programming activity, perhaps based in rhetoric’s roots as a practical art that embraces theory as well as techne and craft, must be be articulated in order to demonstrate that programming is a knowledge-generating, epistemological activity. Along those lines, Malcolm McCullough observes that

> As we overcome the residual notion that computing is for objective documentation only, we
> must cultivate expressive sensibilities. These may result in a digital aesthetic or
> poetics.... And in the end, chances are that appropriate artifacts and descriptions will engage
> us through rich and transparent tools, built on newfound densities of symbolic notation and
> personally experienced as a medium. (1996, 219)

A digital rhetoric that would account for the intellectual work of programming (i.e., the dense symbolic notation that McCullough anticipates) has yet to emerge in the digital humanities. Ramsay and Rockwell’s emphasis on a literary type of theorization privileges an established type of knowledge making, one that is not necessarily welcoming to screen artifacts or the source code behind them. The screen artifact struggles to demonstrate the intellectual work of programming, perhaps they are objects for literary-style analysis by media historians and critics. Software studies is an emerging field that similarly applies literary methods, such as close reading, to the analysis of source code. It’s challenging to distinguish the intellectual work of creation when analytical modes are so well established in the humanities--even if their objects of analysis are relatively new.

Complicating matters, the “personal experience” of a medium that McCullough calls for is preempted by the ossifying tradition of outsourcing what could otherwise be knowledge-making work in the digital humanities. Outsource programming activity to third-party programmers, WYSIWYG interfaces, or readymade software packages like WordPress and Drupal, and it becomes even more difficult to realize McCullough’s calls for something as lofty as a digital aesthetic or poetics rooted in the symbolic materiality of programming.

For those of us who program as a crucial part of our research agendas, then, our argument must proceed by demonstrating that programming *as an activity* is genuine, humanistic inquiry that resists denigration with regard to more established knowledge-making activities grounded in the manipulation and interpretation of symbols.

The need for that line of argument draws writers- and humanists-as-programmers in close company to the knowledge-making practices of art and design. In an obscure but important pamphlet published by the Royal College of Art, Christopher Frayling (1993/4) urges differentiating between three craft-/activity-oriented modes of inquiry: research *into* art and design; research *for* art and design; and research *through* art and design.

Rhetoric and writing, as a humanistic example, have no small body of work that researches *into* writing, often by studying writers and their contexts, such as introductory writing students in first-year composition or seasoned technical writers working in industry. The research conducted *for* writing often takes a pedagogical turn: this line of inquiry is aimed at making writing more teachable to students, rather than necessarily to improve the practice of writing itself.

But it is Frayling’s last prepositional category, research *through* writing and rhetoric—or as I am arguing, *through* programming as “personally experienced” symbolic activity—that remains an underexplored mode of inquiry.

## Magic & Programming

Decades before Steve Jobs introduced to the world the iPad and proclaimed it to be a magical device, Arthur C. Clarke had already articulated what has become known as Clarke’s Third Law: “Any sufficiently advanced technology is indistinguishable from magic.” It is no feat of imagination to see the magic inherent in 64-bit color depths, multitouch interfaces, retina displays, and other hardware-based wonders of screens introduced over the last decade.

To program and to write is to act and create knowledge in the realm of the symbolic. In *Magic, Rhetoric, and Literacy*, William Covino writes that “making language has long been regarded as, in some sense, magical; as a *spell*,” adding “spelling, even in its ostensibly nonmagical sense, denotes the visible materialization of invisible thought” (1994, 5).

The apparently magical incantation of words written in one programming language or another is what makes the symbolic activity of programming a particularly interesting problem for rhetoric and the digital humanities, even when the ends of such activity is visual. Emerging production methods such as responsive web design (RWD; see Marcotte 2010) provide compelling evidence that the written word can trump readymade visual production interfaces in opening up the affordances of newer screens, while still accommodating the old.

Reflecting on the scene from *The Matrix* in which Neo announces to Tank from inside the Construct that he needs “guns, lots of guns,” digital designer John Maeda describes “the sense of magic that occurs when Neo expresses his wish. The instantaneous rush of tremendous resources, as visualized in the simple special effect of this scene, epitomizes for me the experience of freedom when programming the invisible spaces of computer codes” (2004, 17).

While Maeda personally experiences “freedom,” of course, other people no doubt experience the fear inherent in contemplating the magical symbolic activity of programming. “Fear of magic has always been with us, in particular the fear of magic words...which claim to define or alter reality” (Covino 1994, 1). It’s arguably a cultural reflection of this kind of fear that *The Matrix* is set in a simulated reality created by source code that is made visible: to enter the matrix, the camera must pass through streams of code in the film’s opening sequence.

In addition to favoring literary modes of inquiry that I noted above, the digital humanities has inherited a cultural mythos of programming as a mysterious and magical activity. That mythos is probably reinforced by the intercession of so many screens and interfaces that provide both a sanctioned visual kind of magic (the GUI) and tacit promises of protection from a disruptive, unpredictable textual kind of magic (programming).

Covino’s treatment accounts for precisely those two oppositional senses of magic: as “arresting magic,” programming would indeed by conjured only by a particular magus, the programmer, whose spells and incantations (realized in visual interfaces from word processors to smart phones) represent “the imposition of the powerful few upon the unquestioning many” (1994, 8). However, magic presents itself in another sense: “the practice of disrupting and critiquing articulate power: a (re)sorcery of spells for generating multiple perspectives.” Noting that “generative magic enters the world it questions,” Covino argues that generative magic is therefore “an amplification of the possibilities for action” (8).

How are digital humanists, such as digital writers, to discover the possibilities for action such as inquiry, if not through extended personal encounters with programming that “enters the world it questions”? Situated as I am in the study of digital rhetoric, design, and development, this is the digital humanities that I envision: research *through* programming, as a kind of generative magic, that creates knowledge that pushes the digital humanities toward a theory of symbolic action at the source level.

## Model-View-Controller Architecture

Not only have the syntaxes of programming languages evolved, but so too have the implementations of particular paradigms and idiomatic forms within given languages and frameworks. To conclude this chapter, I want to provide a brief look at a specific software architecture, model-view-controller (MVC), as implemented in the Ruby on Rails framework.

MVC is a software design pattern that abstracts and distinguishes three core components of any digital system controlled, importantly, by a graphical user interface. Originally conceived at Xerox PARC by Trygve Reenskaug and his colleagues in the late 1970s, MVC was intended to “to bridge the gap between the human user’s mental model and the digital model that exists in the computer” (Reenskaug 2008). The View provides a visual interface to data described by the Model. The Controller exists to respond to actions occurring with in the View and makes requests to the Model.

Each of MVC’s components must be constructed through programming. Rails provides a number of commands to construct the component parts of MVC from the command line, using the `rails generate` command. `rails generate` is invoked so frequently in Rails that it has been aliased to the shorter `rails g` command. Every Rails tutorial begins with the `rails generate scaffold` command, which produces a basic model, a controller that handles standard create/read/update/delete (CRUD) operations that are typical for working on data, and a set of matching views. In Rails, each view is named with regard to its corresponding controller action.

So to return to the skeletal BeSocial app that I created earlier in the chapter: regardless of what the BeSocial app enables users to do, it is clear that there will need to be users in the system. So the first scaffold that I will create is for a User model, and its corresponding properties (a username, first and last names, and a bio):

    $ rails g scaffold User username:string firstname:string lastname:string bio:text

This line specifies a model called User, that will consist of a username as well as first and last names, each of the string datatype (a string is just a collection of roughly 255 characters), plus a biography, `bio`, that is of the text datatype (basically a much longer string). Rails, in a reflection of Maeda’s observation of the “rush of tremendous resources” called forth from programming, will output something like the following when that command is run (I have isolated just the lines of output that are relevant to this chapter):

      invoke  active_record
      create    app/models/user.rb
      invoke  resource_route
       route    resources :users
      invoke  scaffold_controller
      create    app/controllers/users_controller.rb
      invoke    erb
      create      app/views/users
      create      app/views/users/index.html.erb
      create      app/views/users/edit.html.erb
      create      app/views/users/show.html.erb
      create      app/views/users/new.html.erb
      create      app/views/users/_form.html.erb

Based on one command, Rails has generated this particular scaffold according to my specifications for the data that will make up the User model. By invoking ActiveRecord, Rails’s native Object-Relational Mapping (ORM) module, it has created a recipe (called a *migration*) that specifies how the User object will be mapped to a database table. But unlike Drupal and WordPress, which have traditionally specified a specific database (MySQL), Rails is equipped to connect to and create in many different databases the tables specified in the app. By default, Rails uses an embedded database called SQLite; this is helpful in development, as there are no usernames, passwords, or special connection instructions required for the SQLite database.

The Model code that Rails has generated in the `app/models/user.rb` file is quite minimal:

    # app/models/user.rb
    class User < ActiveRecord::Base
      attr_accessible :bio, :firstname, :lastname, :username
    end
    
Just three lines that define the User class, and allow throughout the rest of Rails access to the four attributes that I specified. If someone wishes to show the record for a particular user, this portion of the controller code would be invoked (I have omitted the other CRUD methods):

    # app/controllers/users_controller.rb
    class UsersController < ApplicationController
      
      # GET /users/1
      # GET /users/1.json
      def show
        @user = User.find(params[:id])

        respond_to do |format|
          format.html # show.html.erb
          format.json { render json: @user }
        end
      end

    end

The line that reads `@user = User.find(params[:id])` is the controller speaking to the model, asking it to create an instance of the User class, based on a particular user ID that is pulled from a URL pattern, e.g., `http://localhost:3000/users/123` will attempt to look for a user with 123 as a unique identifier.

The `@user` instance is in turn available in the user show view; to output the given user’s username in the view, `show.html.erb` would include lines similar to this:

    # app/views/users/show.html.erb
    <p>
      Your username is <%= @user.username %>.
    </p>

The unusual `.html.erb` extension reveals that this template file is written in Embedded Ruby (ERB). Similar to PHP and its `<?php /* Some PHP Code */ ?>` tags that can be inserted alonside regular HTML tags, ERB requires placing Ruby code that is to be output inside of `<%=` and `%>` tags. In this case, the view calls upon the `@user` instance provided by the controller, and the `username` method defined in the model, which is accessed via dot notation: `@user.username`.

Rendered in the browser, that particular line of code for a username `johnsmith` would look something like this, if one chose View > Source from within the web browser:

    <!-- HTML source output at /users/123 -->

    <p>
      Your username is johnsmith.
    </p>

All of this readymade source code, spread among a preplanned set of files and directories, may appear to contradict my earlier complaints about outsourcing programming concerns to frameworks. However, the `rails g scaffold` command serves primarily a pedagogical purpose: it illustrates both how Rails organizes an application (everything of interest here has been created inside of an `app/` directory, with `models/`, `views/`, and `controllers/` each receiving subdirectories within `app/`). It also highlights not just the MVC approach to development, but two additional principles: convention over configuration, and don’t repeat yourself (DRY).

Rails developers typically prefer to use either the stand-alone generators for models and controllers (the latter also generates corresponding views, by default) or, in the case of more advanced developers, custom generators of their own. Rails emphasizes convention over configuration: that is, when some particular pattern (such as that output by `rails g scaffold`) is very likely to be used in an application, that is the pattern it implements. But it is also possible to configure, that is, to do customized work by working with `rails g model` or `rails g controller` for models and controllers, respectively. If one were to create an app that mimics Twitter, for example, it would be unnecessary to have controller actions for updating (Twitter posts can be created or deleted, but not edited or updates). The `edit` and `update` controller actions supplied by `rails g scaffold`, in other words, would be unnecessary. While they could be deleted from the controller file, it’s preferable not to create such actions in the first place if it’s clear at the outset that they’ll never be used.

When I teach Rails in my course on Web Application Development, students and I build one or two throw-away apps using `rails g scaffold`--just to get a sense of how Rails apps are organized, and to illustrate the interactions between the model, a controller action, and the controller action’s corresponding view. When students begin to work on their first serious app, they begin by generating just the models for their application. With those in place, a second Rails command, `rails console`, opens a read-evaluate-print loop (REPL) that has loaded their Rails app. Students then can learn to manipulate the models writing code that would likely appear in their controllers. They can also learn to create methods in their models (such as combining, for example, a `firstname` and `lastname` record into a new method called `fullname`) and test them in the REPL, before attempting to call them from within the Rails app.



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

