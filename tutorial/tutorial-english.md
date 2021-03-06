<!DOCTYPE html>
<html lang="en">
<head>
	
</head>
<body>


<h1>Discipulus's step by step tutorial on module creation with tests and git</h1>



<a href="#dayzero"><h4>day zero: introduction</h4></a>
<ul>
	<li>
		 <a href="#foreword">foreword</a>  
	</li>
	<li>
		 <a href="#thebagoftools">the bag of tools</a>  
	</li>
	<li>
		 <a href="#theplan">the plan</a>  
	</li>
</ul>

	
	

<a href="#dayone"><h4>day one: prepare the ground</h4></a> 
<ul>
	<li>
		 <a href="#dayonestep1">step 1) an online repository on github</a>  
	</li>
	<li>
		 <a href="#dayonestep2">step 2) a new module with module-starter</a>  
	</li>
	<li>
		 <a href="#dayonestep3">step 3) a local repository with git</a>  
	</li>
	
</ul>
	
	
	
	

<a href="#daytwo"><h4>day two: some change and tests</h4></a>
<ul>
	<li>
		 <a href="#daytwostep1">step 1) POD documentation</a>  
	</li>
	<li>
		 <a href="#daytwostep2">step 2) first test</a>  
	</li>
	<li>
		 <a href="#daytwostep3">step 3) commit changes with git</a>  
	</li>
	<li>
		 <a href="#daytwostep3">step 4) pushing to github repository</a>  
	</li>
</ul>

	

<a href="#daythree"><h4>day three: finally some code</h4></a>
<ul>
	<li>
		 <a href="#daythreestep1">step 1) first lines of code</a>  
	</li>
	<li>
		 <a href="#daythreestep2">step 2) testing on our own</a>  
	</li>
	<li>
		 <a href="#daythreestep3">step 3) add dependencies in Makefile.PL</a>  
	</li>
	<li>
		 <a href="#daythreestep4">step 4) run the new test</a>  
	</li>
	<li>
		 <a href="#daythreestep5">step 5) commit, add new files and push with git</a>  
	</li>
</ul>


<a href="#dayfour"><h4>day four: the PODist and the coder</h4></a>  
<ul>
	<li>
		 <a href="#dayfourstep1">step 1) the educated documentation</a>  
	</li>
	<li>
		 <a href="#dayfourstep2">step 2) git status again and commit again</a>  
	</li>
	<li>
		 <a href="#dayfourstep3">step 3) more code...</a>  
	</li>
	<li>
		 <a href="#dayfourstep4">step 4) ...means more and more tests</a>  
	</li>
	<li>
		 <a href="#dayfourstep5">step 5) git: a push for two commits</a>  
	</li>
</ul>


	

<a href="#dayfive"><h4>day five: deeper tests</h4></a>
<ul>
	<li>
		 <a href="#dayfivestep1">step 1) more validation in the code</a>  
	</li>
	<li>
		 <a href="#dayfivestep2">step 2) a git excursus</a>  
	</li>
	<li>
		 <a href="#dayfivestep3">step 3) add deeper tests</a>  
	</li>
	<li>
		 <a href="#dayfivestep4">step 4) who is ahead? git branches and log</a>  
	</li>
	<li>
		 <a href="#dayfivestep5">step 5) overall check and release</a>  
	</li>
	<li>
		 <a href="#dayfivestep6">step 6) test list form</a>  
	</li>
</ul>
	

<a href="#daysix"><h4>day six: testing STDERR</h4></a>
<ul>
	<li>
		 <a href="#daysixstep1">step 1) the problem of empty lists</a>  
	</li>
	<li>
		 <a href="#daysixstep2">step 2) adding a Carp to the lake</a>  
	</li>
	<li>
		 <a href="#daysixstep3">step 3) prepare the fishing road: add a dependency for our test</a>  
	</li>
	<li>
		 <a href="#daysixstep4">step 4) go fishing the Carp in our test</a>  
	</li>
	<li>
		 <a href="#daysixstep5">step 5) document the new warning feature</a>  
	</li>
</ul>	
	
		

<a href="#dayseven"><h4>day seven: the module is done but not ready</h4></a>
<ul>
	<li>
		 <a href="#daysevenstep1">step 1) sharing</a>  
	</li>
	<li>
		 <a href="#daysevenstep2">step 2) files in a CPAN distribution</a>  
	</li>
	<li>
		 <a href="#daysevenstep3">step 3) another kind of test: MANIFEST</a>  
	</li>
	<li>
		 <a href="#daysevenstep4">step 4) another kind of test: POD and POD coverage</a>  
	</li>
	<li>
		 <a href="#daysevenstep5">step 5) some README and final review of the work</a>  
	</li>
	<li>
		 <a href="#daysevenstep6">step 6) try a real CPAN client installation</a>  
	</li>
</ul>	


	
	
<a href="#dayeight"><h4>day eight: other module techniques</h4></a>
<ul>
	<li>
		 <a href="#dayeightoptionone">option one - the bare bone module</a>  
	</li>
	<li>
		 <a href="#dayeightoptiontwo">option two - the Exporter module</a>  
	</li>
	<li>
		 <a href="#dayeightoptionthree">option three - the OO module</a>  
	</li>
	<li>
		 <a href="#dayeightothertestingmodules">other testing modules</a>  
	</li>
	<li>
		 <a href="#dayeightadvancedMakefile.PLusage">advanced Makefile.PL usage</a>  
	</li>
	<li>
		 <a href="#dayeightadvancedtestingcode">advanced testing code	</a>  
	</li>
</ul>


<a href="#bibliography"><h4>bibliography</h4></a>	
<ul>
	<li>
		 <a href="#COREdocumentationaboutmodules">CORE documentation about modules</a>  
	</li>
	<li>
		 <a href="#COREdocumentationabouttesting">CORE documentation about testing</a>  
	</li>
	<li>
		 <a href="#furtherreadingsaboutmodules">further readings about modules</a>  
	</li>
	<li>
		 <a href="#furtherreadingsabouttesting">further readings about testing</a>	
	</li>
</ul>

<a href="#acknowledgements"><h4>acknowledgements</h4></a>



	
<a id="dayzero"></a>
<h2>day zero: introduction</h2>



<a id="foreword"></a>
<h4>foreword</h4>

This tutorial is not about coding: that's it! The code, idea and implementation presented below
are, by choice, futile, piffling and trifling ( the module resulting following this tutorial is available, archived <a href="https://github.com/LorenzoTa/Range-Validator">on its own repository</a>).

This tutorial, by other hands, tries to show to the beginner one possible path in module creation. As always in perl there are many ways to get the job done and mine is far to be the optimal one, but as
I have encountered many difficulties to choice my own path, perhaps sharing my way can help someone else.

There are other similar but different source of knowledge about module creation, notably <a href="https://www.perlmonks.org/index.pl?node_id=431702">José's Guide for creating Perl modules</a>: read this for some point i do not explore (well, read it anyway: it's worth to)



<a id="thebagoftools"></a>
<h4>the bag of tools</h4>

As for every duty, check your equipment before starting. You probably already have perl, a shell (or something less fortunate if you are on windows, like me ;) and a favourite text editor or IDE.

But here in this tutorial we'll use  <code>git</code> in the command line and <a href="https://github.com">github</a> to store our work in a central point (very handy feature). So get a <code>github</code> account and a <code>git</code> client.

This tutorial will focus on the importance (I'd say preminence or even predominance) of testing while developing a perl module. I wrote lonely scripts for years then I realized that even if my script seemed robust, I have no way to test them in a simple and reliable way.

So we will use the core module <a href="http://perldoc.perl.org/Test/More.html">Test::More</a> and the CPAN one <a href="https://metacpan.org/pod/Test::Exception">Test::Exception</a> in our module so get it installed using your <code>cpan</code> or <code>cpanm</code> client. Take a look to <a href="http://perldoc.perl.org/Test/Simple.html">Test::Simple</a> if you are not used to test.

We also use the core module <a href="http://perldoc.perl.org/Carp.html">Carp</a> to report errors from user point of view.

We use <a href="https://metacpan.org/pod/Module::Starter">Module::Starter</a> to have the skeleton of our module done for us, but, as always there are valid alternatives. Install it.

We'll document our module using POD (Plain Old Documentation) see <a href="https://perldoc.perl.org/perlpod.html">perlpod</a> for reference.



<a id="theplan"></a>
<h4>the plan</h4>


Some of your programs or modules work on lists and arrays. Functions inside these programs accept ranges but while you intend what a valid ranges is ( <code>0,1,2</code> or <code>0..2</code> ) you discover that your programs crashed many times because other humans or other programs passed ranges like: <code>0,1..3,2</code> (where <code>2</code> is present twice) or <code>3,2,1</code> (and your application is silently expecting <code>1,2,3</code> ) or <code>9..1</code> or even <code>0,1,good,13..15</code> not being a range at all, or simply <code>1-3</code> being a range for the user but not for you perl code that read it as <code>-2</code>.

Bored of the situation you plan a new module to validate ranges. <code>Range::Validator</code> is the name you choose. Your initial plan is to expose just one sub: <code>validate</code>

As in masonry, you need a well prepared plan before starting excavations. Then you need points and lines drawn on the terrain: everything that makes the job complex is part of the job itself.

Look around: you can
bet someone else got your same idea before you. You can also bet he or she was smarter than you and it already uploaded it to <a href="https://metacpan.org">CPAN</a>. 

Sharing early is a good principle: if you already have an idea of your module (even before implementing it), can be worth to ask in a forum dedicated to Perl (like <a href="https://www.perlmonks.org">perlmonks.org</a>) posting a RFC post (Request For Comments) or using  the dedicated website <a href="http://prepan.org/ ">prepan.org</a>(is not a crowdy place nowadays..;).

Plan it well: it is difficult, but remember that to repair something bad planned is always a worst task.
The basic read is in the core documentation: <a href="http://perldoc.perl.org/index-language.html">perlnewmod</a> is the place to start and <a href="http://perldoc.perl.org/perlmodstyle.html">perlmodstyle</a> is what comes next. Dont miss the basic documentation. 

If you want to read more see, in my <a href="https://www.perlmonks.org/index.pl?node_id=1202418#modules">bibliotheca</a>, the scaffold dedicated to modules.

Choose carefully all your names: the module one and names of methods or functions your module exports: good code with bad named methods is many times unusable by others than the author.


Programming is a matter of interfaces. sic. dot. Coding is easy engineering is hard. sic. another dot.
You can change a million of times the implementation, you can never change how other people use your code. So plan well what you offer with your module. You can add in the future new features; you cannot remove not even one of them because someone is already using it in production. Play nice: plan well.

You can profit the read of a wonderful post: <a href="https://www.perlmonks.org/index.pl?node_id=553487">
On Interfaces and APIs</a>






<a id="dayone"></a>
<h2>day one: prepare the ground</h2>


<a id="dayonestep1"></a>
<h4>step 1) an online repository on github</h4> 

Create an empty repository on the github server named Range-Validator (they do not accept <code>::</code> in names) see <a href="https://help.github.com/articles/creating-a-new-repository/">here for instruction</a>

<a id="dayonestep2"></a>
<h4>step 2) a new module with module-starter</h4>

Open a shell to your scripts location and run the program <code>module-starter</code> that comes within <code>Module::Starter</code> It wants a  mail address, the author name and, obviously the module name:

<pre>
shell> module-starter --module Range::Validator --author MyName --email MyName@cpan.org

Added to MANIFEST: Changes
Added to MANIFEST: ignore.txt
Added to MANIFEST: lib/Range/Validator.pm
Added to MANIFEST: Makefile.PL
Added to MANIFEST: MANIFEST
Added to MANIFEST: README
Added to MANIFEST: t/00-load.t
Added to MANIFEST: t/manifest.t
Added to MANIFEST: t/pod-coverage.t
Added to MANIFEST: t/pod.t
Added to MANIFEST: xt/boilerplate.t
Created starter directories and files

</pre>
A lot of work done for us! The <code>module-starter</code> program created all the above files into a new folder named <code>Range-Validator</code> let's see the content:

<pre>
---Range-Validator
   |   Changes
   |   ignore.txt
   |   Makefile.PL
   |   MANIFEST
   |   README
   |
   |---lib
   |
   |    ---Range
   |           Validator.pm
   |
   |----t
   |       00-load.t
   |       manifest.t
   |       pod-coverage.t
   |       pod.t
   |
   |----xt
           boilerplate.t
</pre>
We now have a good starting point to work on. Spend some minute to review the content of the files to get an idea.






<a id="dayonestep3"></a>
<h4>step 3) a local repository with git</h4> 

Open another shell for the git client (I prefer to have two, feel free to use just one) to the same path of the above created folder and initialize a git repository (local for the moment) there:

<pre>
git-client> git init

Initialized empty Git repository in /path/to/Range-Validator/.git/

</pre>
Nothing  impressive.. What happened? The above command created a <code>.git</code> directory, ~15Kb of infos, to take track of all changes you'll make to your files inside the <code>Range-Validator</code> folder. In other words it created a git repository. Empty. Empty?!? And all my files?

It's time for a command you'll use many, many times: <code>git status</code>

<pre>
git-client> git status

On branch master

No commits yet

Untracked files:
  (use "git add &lt;file&gt;..." to include in what will be committed)

        Changes
        MANIFEST
        Makefile.PL
        README
        ignore.txt
        lib/
        t/
        xt/

nothing added to commit but untracked files present (use "git add" to track)
</pre>
Many terms in the above output would be worth to be explained, but not by me. Just be sure to understand what <code>branch</code>, <code>commit</code>, <code>tracked/untracked</code> means in the git world. Luckily the command is so sweet to add a hint for us as last line: <code>(use "git add" to track)</code> 

Git is built for this reason: it can track all modifications we do to code base and it take a picture (a snapshot in git terminology) of the whole code base everytime we commit these changes. But <code>git init</code> initialized an empty repository: we must tell git which files to add to tracked ones.

We simply want to track all files <code>module-starter</code> created for us: <code>git add .</code> add the current directory and all its content to tracked content. Run it and check the status again:

<pre>
git-client> git add .

git-client> git status

On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached &lt;file&gt;..." to unstage)

        new file:   Changes
        new file:   MANIFEST
        new file:   Makefile.PL
        new file:   README
        new file:   ignore.txt
        new file:   lib/Range/Validator.pm
        new file:   t/00-load.t
        new file:   t/manifest.t
        new file:   t/pod-coverage.t
        new file:   t/pod.t
        new file:   xt/boilerplate.t

</pre>
We added all content but we still have not committed anything! <code>git commit -m "some text"</code> will commit all changes using the message provided as a label for the commit (without <code>-m</code> git will open a text editor to enter the text). Run it and recheck the status again:

<pre>
git-client> git commit -m "module-starter created content"

[master (root-commit) 1788c12] module-starter created content
 11 files changed, 409 insertions(+)
 create mode 100644 Changes
 create mode 100644 MANIFEST
 create mode 100644 Makefile.PL
 create mode 100644 README
 create mode 100644 ignore.txt
 create mode 100644 lib/Range/Validator.pm
 create mode 100644 t/00-load.t
 create mode 100644 t/manifest.t
 create mode 100644 t/pod-coverage.t
 create mode 100644 t/pod.t
 create mode 100644 xt/boilerplate.t


git-client> git status

On branch master
nothing to commit, working tree clean

</pre>
With the above we committed everything. The status is now <code>working tree clean</code> what better news for a lumberjack used to examine daily tons of dirty logs? ;)


Now we link the local copy and the remote one on github: all examples you find, and even what github propose to you, tell <code>git remote add origin https://github.com/...</code> where <code>origin</code> is not a keyword but just a label, a name: I found this misleading and I use my github name in this place or something
that tell me the meaning, like <code>MyFriendRepo</code>. So from now on we will use <code>YourGithubLogin</code> there.

Add the remote and verify it ( with <code>-v</code> ):
<pre>
git-client> git remote add YourGithubLogin https://github.com/YourGithubLogin/Range-Validator.git

git-client> git remote -v

YourGithubLogin       https://github.com/YourGithubLogin/Range-Validator.git (fetch)
YourGithubLogin       https://github.com/YourGithubLogin/Range-Validator.git (push)

</pre>
The verify operation gives us two hints: for the remote repository that we call <code>YourGithubLogin</code> we can do <code>fetch</code> (import all changes you still have not, from the remote repository to your local copy) or <code>push</code> (export your local copy to the remote repository).

Since on github there is nothing and locally we have the whole code base, we definitively want to <code>push</code> and we can do that if and only if, we have the permission in the remote repository. It's our own repository, so no problem (git will ask for the github password). The <code>push</code> wants to know which branch to push: we only have <code>master</code> so:

<pre>
git-client> git push YourGithubLogin master

fatal: HttpRequestException encountered.
   
Username for 'https://github.com': YourGithubLogin
Password for 'https://YourGithubLogin@github.com': ***********

Counting objects: 17, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (14/14), done.
Writing objects: 100% (17/17), 5.33 KiB | 303.00 KiB/s, done.
Total 17 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/YourGithubLogin/Range-Validator/pull/new/master
remote:
To https://github.com/YourGithubLogin/Range-Validator.git
 * [new branch]      master -> master
</pre>
Go to the github website to see what happened: the whole code base is in the online repository too, updated to our last commit (aka our first, unique commit for the moment). From now on we can work on our code from any machine having a <code>git</code> client. To do so we must be diligent and committing and pushing our changes when is the moment, to maintain the online repository up to date. Clean yard, happy master mason.

A whole day is passed, well.. two days, and we did not wrote a single line of perl code: we are starting the right way! Time to go to sleep with a well prepared playground.



<a id="daytwo"></a>
<h2>day two: some change and tests</h2>


<a id="daytwostep1"></a>
<h4>step 1) POD documentation</h4> 

Well first of all some cleaning: open you local copy of the module <code>/path/to/Range-Validator/lib/Range/Validator.pm</code> in your text editor or IDE. Personally  I like the POD documentation to be all together after the <code>\_\_DATA\_\_</code> token rather interleaved with the code. Inside the code I only like to have comments. POD documentation is for the user, comments are for you! After a week or month you'll never remember what your code is doing: comment it explaining what is passing.

So go to the end of the module where the line is the final <code>1;</code> ( remember all modules must have a true return value as last statement) and place, in a new line the <code>\_\_DATA\_\_</code> token. Move all POD after the token. Also cancel the POD and the code relative to <code>function2</code>

Then rename <code>function1</code> into <code>validate</code> and change accordingly the name of the POD section too.

Modify the POD part <code>=head1 NAME</code> with a more humble and meaning description: <code>Range::Validator - a simple module to verify array and list ranges</code>

Change the <code>=head1 SYNOPSIS</code> part too, removing unneeded text and changing code lines ( see below ): we do not do an object oriented module, so no <code>new</code> method for us. You plan to accept both real ranges and strings representing ranges.

So, if you followed me, the module must look like:
<pre>
package Range::Validator;

use 5.006;
use strict;
use warnings;

our $VERSION = '0.01';

sub validate {
}

1;

__DATA__

=head1 NAME

Range::Validator - a simple module to verify array and list ranges

=head1 VERSION

Version 0.01

=cut

=head1 SYNOPSIS

    use Range::Validator;

    my @range = Range::Validator->validate(0..3);      # a valid range
	
	my @range = Range::Validator->validate(0..3,2);    # a overlapping range
	
	my @range = Range::Validator->validate('1,3,7');   # a valid range passed as a string
    
	my @range = Range::Validator->validate('1,XXX,3'); # an invalid range  passed as a string
	
# more POD ...

</pre>
Ok? Let's check our new POD is correct: open the shell in the directory created yesterday <code>/path/to/Range-Validator</code> and run the following command: <code> perldoc ./lib/Range/Validator.pm </code> 

Review the POD. It must be ok. 


<a id="daytwostep2"></a>	
<h4>step 2) first test</h4> 

Now we test if the module syntax is correct. The first simple method is a short one liner using the perl option <code> -I </code> to include <code>./lib</code> in <code>@INC</code> and <code> -MRange::Validator </code> to use our module( see <a href="https://perldoc.perl.org/perlrun.html">
perlrun</a> and <a href="https://perldoc.perl.org/perlvar.html">
perlvar</a> ):

<pre>
shell> perl -I ./lib -MRange::Validator -e 1

shell>
</pre>
No errors: good! the module can be used and has no syntax errors. But.. one moment: we want to try out all our features, and we plan to add many, using one liners? Are we mad?! No; we will use tests. 

Tests are wonderful in perl and planning good tests (a test suite) will save a lot of time in the future and makes your code maintainable. The time you invest writing tests <b>while coding</b> will save a lot of time in the future when you modify the code base. I'm not a theoric of software writing nor an orthodox of test driven development, but to write tests while you code is a very good practice. You can even write tests <b>before coding</b> ie: you write something that test a wanted behaviour, you run it expecting a failure, then you write the code that make the test happy. This is up to you.

What is not a choice is having no test suite or writing all tests at the end of code development. No.

In the day one we used <code>module-starter</code> to produce a skeleton of our module. <code>module-starter</code> was so kind to write a bounch of tests for us in the standard directory <code>/t</code> (ie tests). Tests are run normally during the installation (sorted by their names) of the module but, as we already said, they are the main source of serenity for us as developers. So let's see what <code>module-starter</code> wrote inside <code>/t/00-load.t</code>

<pre>
#!perl -T
use 5.006;
use strict;
use warnings;
use Test::More;

plan tests => 1;

BEGIN {
    use_ok( 'Range::Validator' ) || print "Bail out!\n";
}

diag( "Testing Range::Validator $Range::Validator::VERSION, Perl $], $^X" );

</pre>
This perl program use strict and wanrings (you already know they are friends, do you?) then load the core module <a href="https://perldoc.perl.org/Test/More.html">Test::More</a> which generally
requires that you declare how many tests you intend to run ( <code>plan tests => 1</code> ) then inside the <code>BEGIN</code> block use its method <code>use_ok</code> that loads our own module and in case of failure print "Bail out!\n" aka "everything went wrong, leave the boat".

If the above succeeded <a href="https://perldoc.perl.org/Test/More.html">Test::More</a> calls <code>diag</code> that emits a note with the text specified, useful to have while reviewing test output. The module also has the <code>note</code> method that I prefer. Go to the module documentation to have an idea of <a href="https://perldoc.perl.org/Test/More.html">Test::More</a>

So, instead of the one liner we can safely call this test:

<pre>
shell> perl -I ./lib ./t/00-load.t

"-T" is on the #! line, it must also be used on the command line at ./t/00-load.t line 1.

</pre>
The test crash because of the <code>-T</code> that turns taint mode on. Taint mode is base of the security in perl, but for the moment we do not need it enabled, so we remove from the shebang line which will result in <code>#!perl</code> (read about taint mode in the official perl documentation: <a href="https://perldoc.perl.org/perlsec.html#Taint-mode">perlsec</a>). 

(Note that removing <code>-T</code> switch is not the best thing to do: <code>perl -T -I ./lib ./t/00-load.t</code> is by far a better solution).

After this change the test will run as expected:

<pre>
shell> perl -I ./lib ./t/00-load.t

ok 1 - use Range::Validator;
1..1
# Testing Range::Validator 0.01, Perl 5.026000, /path/to/my/perl

</pre>
Wow! we run our first test! ..yes, but in the wrong way. Well not exactly the wrong way but not the way tests are run during installation.
Test are run through a TAP harness (TAP stands for Test Anything Protocol and is present in perl since ever: perl born the right way ;).

With your perl distribution you have the <a href="https://perldoc.perl.org/prove.html">prove</a> command (see its documentation) that run tests through a TAP harness. So we can use it.

We can call <a href="https://perldoc.perl.org/prove.html">prove</a> the very same way we called perl: <code>prove -I ./lib ./t/00-load.t</code> but we are lazy and we spot <code>prove -l</code> which has the same effect of <code>prove -I ./lib</code> ie include <code>./lib</code> in <code>@INC</code>

Run the very same test through <a href="https://perldoc.perl.org/prove.html">prove</a> instead that perl and you will see a slightly different output:

<pre>
shell> prove -l ./t/00-load.t

./t/00-load.t .. 1/? # Testing Range::Validator 0.01, Perl 5.026000,  /path/to/my/perl
./t/00-load.t .. ok
All tests successful.
Files=1, Tests=1,  0 wallclock secs ( 0.01 usr +  0.02 sys =  0.03 CPU)
Result: PASS

</pre>
Basically the output includes some statistics and the count of test files processed and the overall number of tests. Also note that the message emitted by <code>diag</code> is in another place: diagnostics by <a href="https://perldoc.perl.org/Test/More.html">Test::More</a> goes to <code>STDERR</code> (which is buffered differently in respect of <code>STDOUT</code> but this is another story..) and TAP aggregates tests results and prints them to <code>STDOUT</code>

Finally we have the developer gratification: <code>Result: PASS</code> indicating all went well.

The <code>prove</code> program promotes laziness and without argument (as a test file in the previous example) runs automatically every test file found under <code>/t</code> folder: this is the same behaviour you will have during an effective module installation:

<pre>
shell> prove -l

t\00-load.t ....... 1/? # Testing Range::Validator 0.01, Perl 5.026000, /path/to/my/perl
t\00-load.t ....... ok
t\manifest.t ...... skipped: Author tests not required for installation
t\pod-coverage.t .. skipped: Author tests not required for installation
t\pod.t ........... skipped: Author tests not required for installation
All tests successful.
Files=4, Tests=1,  1 wallclock secs ( 0.06 usr +  0.02 sys =  0.08 CPU)
Result: PASS

</pre>



<a id="daytwostep3"></a>
<h4>step 3) commit changes with git</h4> 

Ok we have done some change to the code base, small ones but changes. Wich changes? I'm lazy and I do not remember all files we modified. No problem <code>git</code> will tell us. At least I remember which command I need to review the code base status: <code>git status</code>

Go to the git shell and run it:

<pre>
git-client> git status

On branch master
Changes not staged for commit:
  (use "git add &lt;file&gt;..." to update what will be committed)
  (use "git checkout -- &lt;file&gt;..." to discard changes in working directory)

        modified:   lib/Range/Validator.pm
        modified:   t/00-load.t

no changes added to commit (use "git add" and/or "git commit -a")

</pre>
Ah yes, we modified two files: not only the module also the <code>t/00-load.t</code> removing the <code>-T</code> from shebang line, thanks <code>git</code> and you are also so kind to give me two hints about what to do next: <code>use "git add" and/or "git commit -a"</code>

Go for the shorter path: we commit adding all files  with <code>git commit -a</code> ie: we commit all files <b>that are already tracked</b> and eventually we remove from tracked list all files deleted in the code base. But we remember that committing needs to include a message as label of the commit:  <code>git commit -m "message"</code> so putting all together and checking the status:

<pre>
git-client> git commit -a -m "moved POD, removed -T"

[master 49a0690] moved POD, removed -T
 2 files changed, 20 insertions(+), 23 deletions(-)
 
git-client> git status

On branch master
nothing to commit, working tree clean
 
</pre>





<a id="daytwostep4"></a>
<h4>step 4) pushing to github repository</h4> 

Ok we submitted, well committed, all changes made. What's next? We have to synchronize the online repository that we named <code>YourGithubLogin</code> so check it and push modified content to it:

<pre>
git-client>git remote -v

YourGithubLogin   https://github.com/YourGithubLogin/Range-Validator (fetch)
YourGithubLogin   https://github.com/YourGithubLogin/Range-Validator (push)


git-client> git push YourGithubLogin master

fatal: HttpRequestException encountered.
   
Username for 'https://github.com': YourGithubLogin
Password for 'https://YourGithubLogin@github.com':
Counting objects: 7, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 870 bytes | 435.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/YourGithubLogin/Range-Validator
   1788c12..49a0690  master -> master

</pre>
Go to the browser and open the online repository to see what happened after the <code>git push</code>: in the main page, where files are listed we spot our two modified files with a new timestamp and with the message we used when committing. Under the Insight tab and then under Network in the right menu, we can see two points connected by a line segment: this is the visual history of our repository and each commit we have done: here you will find also eventual branches, but this is another story.

Well, another day is passed without writing a single line of perl code! At least for the moment our code is 100% bug free ;)
I vaguely recall a chinese motto: "when you start something, start from the opposite" or something like that. To write a robust perl module start writing no perl code, for two days!






<a id="daythree"></a>	
<h2>day three: finally some code</h2>


<a id="daythreestep1"></a>		
<h4>step 1) first lines of code</h4> 

It's time to put some code inside our <code>validate</code> subroutine. We plan to accept both a string like <code>'1..3,5'</code> and a pure range like <code>1..5,6</code> but let's start with string form assuming only one element will be passed to our sub via <code>@_</code>

Remember what said in the foreword: this tutorial is not about coding, so be merciful with following examples.

<pre>
sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
	}
	# otherwise we received a list
	else{
		...
	}	
	return @range;
}

</pre>
The above is straightforward (if ugly): we get something in  via <code>@_</code> (a string or a list) and we return something via <code>return @range</code> To accomplish this we initialize <code>$range</code> to hold our string.

A good principle in loops is "put exit conditions early" and following this principle we put our our die conditions as soon as possible, ie after the if/else check.

But we dont want to die with an ugly message like <code>Died at ../Range/Validator.pm line x</code> ie from the module perspective: we want to inform the user where his code provoked our module to die.

The core module <a href="https://perldoc.perl.org/Carp.html">Carp</a> provides this kind of behaviour and we use its function <code>croak</code> that dies from perspective of the caller.

So we add the line needed to load the module, a first <code>croak</code> call if the string passed in contains forbidden  characters and some other line too:

<pre>
package Range::Validator;

use 5.006;
use strict;
use warnings;

use Carp;									# --- new line

our $VERSION = '0.01';

sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
	}
	# otherwise we received a list
	else{
		...
	}
	# remove any space from string
	$range =~ s/\s+//g;						# --- new line
	# die if invalid characters
	croak "invalid character passed in string [$range]!" 
			if $range =~ /[^\s,.\d]/;		# --- new line
	
	@range = eval ($range);					# --- new line
	return @range;
}

1;
</pre>



<a id="daythreestep2"></a>	
<h4>step 2) testing on our own</h4> 

How to see if all works as expected? Obviously with a test. Not <code>00-load.t</code> but a new one dedicated to the <code>validate</code> sub. So go into the <code>t</code> folder and create a new file <code>01-validate.t</code> and open it to edit the content.

Let's populate it with a basic content plus some new stuff (<code>01-validate.t</code>):

<pre>
#!perl
use 5.006;
use strict;
use warnings;
use Test::More qw(no_plan);
use Test::Exception;

use_ok( 'Range::Validator' ); 

ok (scalar Range::Validator::validate('0..2') == 3, 
	'ok valid string produces correct number of elements' );

note ("starting test of forbidden characters in the string form");

dies_ok { Range::Validator::validate('xxxinvalidstringxxx') }
			"expected to die with invalid character";

</pre>
First of all we used a different notation for <a href="https://perldoc.perl.org/Test/More.html">Test::More</a> ie. <code>use Test::More qw(no_plan)</code> 

We are telling to the module we (still) have not a plan about how many tests will be in this file. This is a handy feature.

The <a href="https://perldoc.perl.org/Test/More.html">Test::More</a> core module offers us <code>ok</code> <code>use_ok</code> and <code>note</code> methods: view the module doc for more info about them.

But we also used in the above test the <code>dies_ok</code> function: this one comes from the CPAN module <code>Test::Exception</code> and we need to add this module in to our dependencies list.

Dependencies list? What is that? Where we spoke about this? Never, until now. 




<a id="daythreestep3"></a>
<h4>step 3) add dependencies in Makefile.PL</h4> 

Infact the program <code>module-starter</code> used in day one created a file called <code>Makefile.PL</code> with the following default content:

<pre>
use 5.006;
use strict;
use warnings;
use ExtUtils::MakeMaker;

WriteMakefile(
    NAME             => 'Range::Validator',
    AUTHOR           => q{MyName &lt;MyName@cpan.org&gt;},
    VERSION_FROM     => 'lib/Range/Validator.pm',
    ABSTRACT_FROM    => 'lib/Range/Validator.pm',
    LICENSE          => 'artistic_2',
    PL_FILES         => {},
    MIN_PERL_VERSION => '5.006',
    CONFIGURE_REQUIRES => {
        'ExtUtils::MakeMaker' => '0',
    },
    BUILD_REQUIRES => {
        'Test::More' => '0',		
    },
    PREREQ_PM => {
        #'ABC'              => '1.6',
        #'Foo::Bar::Module' => '5.0401',
    },
    dist  => { COMPRESS => 'gzip -9f', SUFFIX => 'gz', },
    clean => { FILES => 'Range-Validator-*' },
);

</pre>
This file is run on the target system trying to install your module. It's vaste matter and you can find many, many useful informations in the core documentation of <a href="https://perldoc.perl.org/ExtUtils/MakeMaker.html">ExtUtils::MakeMaker</a> and in the <a href="https://perldoc.perl.org/ExtUtils/MakeMaker/Tutorial.html">ExtUtils::MakeMaker::Tutorial</a> and, as always in perl, there many ways to do it.

In our simple case we only need to know few facts about <code>BUILD_REQUIRES</code> and <code>PREREQ_PM</code> fields.

The first one lists into a hash all modules and their version needed to build up our module, building includes testing, so if you need some module during tests it is the place where insert dependencies. The <code>module-starter</code> program added <code>'Test::More' => '0'</code> entry for us. This is the right place to state that we intend to use <a href="https://metacpan.org/pod/Test::Exception">Test::Exception</a> CPAN module during tests.

By other hand <code>PREREQ_PM</code> lists modules and their minimal versions needed to run your module. As you can see it's a different thing: to run <code>Range::Validator</code> you never need <code>Test::Exception</code> but, for example you 'll need <code>Carp</code>

Even if <code>Carp</code> it's a core module is a good practice to include it into <code>PREREQ_PM</code> 

Read a very good post about dependencies <a href="https://www.perlmonks.org/?node_id=946044">Re: How to specify tests dependencies with Makefile.PL?</a>

Cleaning example lines and given all the above, we will modify <code>Makefile.PL</code> as follow:

<pre>
use 5.006;
use strict;
use warnings;
use ExtUtils::MakeMaker;

WriteMakefile(
    NAME             => 'Range::Validator',
    AUTHOR           => q{MyName &lt;MyName@cpan.org&gt;},
    VERSION_FROM     => 'lib/Range/Validator.pm',
    ABSTRACT_FROM    => 'lib/Range/Validator.pm',
    LICENSE          => 'artistic_2',
    PL_FILES         => {},
    MIN_PERL_VERSION => '5.006',
    CONFIGURE_REQUIRES => {
        'ExtUtils::MakeMaker' => '0',
    },
    BUILD_REQUIRES => {
        'Test::More' => '0',
		'Test::Exception' => '0',	# --- new line
    },
    PREREQ_PM => {
        'Carp'	=> '0',				# --- new line
    },
    dist  => { COMPRESS => 'gzip -9f', SUFFIX => 'gz', },
    clean => { FILES => 'Range-Validator-*' },
);
</pre>
So the moral is: when you add a dependency needed to run your module or to test it remember to update <code>Makefile.PL</code> correspondent part.



<a id="daythreestep4"></a>
<h4>step 4) run the new test</h4> 
Ok, is the above test ok? It returns all we expect? Try it using <code>prove -l</code> but specifying also <code>-v</code> to be verbose and the filename of our new test (now we dont want all test run, just the one we are working on):

<pre>
shell> prove -l -v ./t/01-validate.t

./t/01-validate.t ..
ok 1 - use Range::Validator;
ok 2 - ok valid string produces correct number of elements
# starting test of forbidden characters in the string form
ok 3 - expected to die with invalid character
1..3
ok
All tests successful.
Files=1, Tests=3,  0 wallclock secs ( 0.05 usr +  0.01 sys =  0.06 CPU)
Result: PASS

</pre>


<a id="daythreestep5"></a>
<h4>step 5) commit, add new files and push with git</h4> 

What we need more from our first day of coding? To check our status and to synchronize our online repository (pay attention to the following commands because we have a new, untracked file!):

<pre>
git-client> git status

On branch master
Changes not staged for commit:
  (use "git add &lt;file&gt;..." to update what will be committed)
  (use "git checkout -- &lt;file&gt;..." to discard changes in working directory)

        modified:   Makefile.PL
        modified:   lib/Range/Validator.pm

Untracked files:
  (use "git add &lt;file&gt;..." to include in what will be committed)

        t/01-validate.t

no changes added to commit (use "git add" and/or "git commit -a")

git-client> git commit -a -m "some code into validate and modified Makefile.PL"

[master 580f628] some code into validate and modified Makefile.PL
 2 files changed, 23 insertions(+), 3 deletions(-)

</pre>
We committed before adding the new file! shame on us! Add the new file and issue another commit:

<pre>
git-client> git add  t/01-validate.t


git-client> git status

On branch master
Changes to be committed:
  (use "git reset HEAD &lt;file&gt;..." to unstage)

        new file:   t/01-validate.t

git-client> git commit -a -m "added 01-validate.t"

[master 5083ec3] added 01-validate.t
 1 file changed, 16 insertions(+)
 create mode 100644 t/01-validate.t

git-client> git status

On branch master
nothing to commit, working tree clean

</pre>
What more? Ah! pushing to the online repository:
<pre>
git-client> git remote -v

YourGithubLogin   https://github.com/YourGithubLogin/Range-Validator (fetch)
YourGithubLogin   https://github.com/YourGithubLogin/Range-Validator (push)

git-client> git push YourGithubLogin master

fatal: HttpRequestException encountered.
  
Username for 'https://github.com': YourGithubLogin
Password for 'https://YourGithubLogin@github.com': *********
Counting objects: 10, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (10/10), 1.31 KiB | 447.00 KiB/s, done.
Total 10 (delta 5), reused 0 (delta 0)
remote: Resolving deltas: 100% (5/5), completed with 4 local objects.
To https://github.com/YourGithubLogin/Range-Validator
   49a0690..5083ec3  master -> master
</pre>
What a day! We added six lines of code and an entire test file! Are we programming too much? Probably no but we are doing it in a robust way and we discovered it can be hard work. In perl hard work is justified only by (future) laziness and we are doing all these work because we are lazy and we do not want to waste our time when, in a month or a year, we need to take this code base again to enhance it or to debug it. So now it's time for the bed and for deserved colorful dreams.





<a id="dayfour"></a>
<h2>day four: the PODist and the coder</h2>


<a id="dayfourstep1"></a>
<h4>step 1) the educated documentation</h4> 

We get up in the morning and we suddenly realize yesterday we forgot something very important: documentation!
Good documentation is like an educated people, while poor documentation is like a boor one: who do you prefer to meet?

The same is for your module users: they hope and expect to find a good documentation and to write it is our duty. Dot.

Documentation content, in my little experience, can be impacted a lot for even small changes in the code or interface so, generally I write the larger part of the docs when the implementation or interface is well shaped. But, by other hand, a good approach is to put in the docs every little statement that will be true since the very beginning of your module development. At the moment we can state our <code>validate</code> sub accepts both strings and ranges and always returns an array.

At the moment the relevant part of the POD documentation is:

<pre>
=head1 EXPORT

A list of functions that can be exported.  You can delete this section
if you don't export anything, such as for a purely object-oriented module.

=head1 SUBROUTINES/METHODS

=head2 validate

=cut

</pre>
We do not plan to export functions: our sub must be called via its fully qualified name, as we do in the test we created: <code>Range::Validator::validate()</code> so we can delete the EXPORT part and add something in the subroutines part:


<pre>
=head1 SUBROUTINES

=head2 validate

This function accepts a string or a list (range) and returns an array.
In the string form the accepted characters are: positive integers, dots, commas and spaces. Every space will be removed.

</pre>
We do not need <code>=cut</code> anymore because we do not have POD in blocks interleaved with the code, but an unique POD block in the <code>\_\_DATA\_\_</code> section.




<a id="dayfourstep2"></a>
<h4>step 2) git status again and commit again</h4> 

Since we are now very fast with <code>git</code> commands, let's <code>commit</code> this little change; the <code>push</code> to the remote repository can be left for the end of work session. So <code>status</code> (check it frequently!) and <code>commit</code>

<pre>
git-client> git status

On branch master
Changes not staged for commit:
  (use "git add &lt;file&gt;..." to update what will be committed)
  (use "git checkout -- &lt;file&gt;..." to discard changes in working directory)

        modified:   lib/Range/Validator.pm

no changes added to commit (use "git add" and/or "git commit -a")


git-client> git commit -a -m "initial POD to document validate function"

[master a6dc557] initial POD to document validate function
 1 file changed, 5 insertions(+), 6 deletions(-)

</pre>



<a id="dayfourstep3"></a>
<h4>step 3) more code...</h4> 

Now it's time to add more checks for the incoming string: we do not accept a lone dot between non dots, nor even more than two dots consecutively:

<pre>
# not allowed a lone .
	croak "invalid range [$range] (single .)!" if $range =~ /[^.]+\.{1}[^.]+/;
# not allowed more than 2 .
	croak "invalid range [$range] (more than 2 .)!" if $range =~ /[^.]+\.{3}/;
		
</pre>
The whole sub now look like:

<pre>
sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
	}
	# otherwise we received a list
	else{
		...
	}
	# remove any space from string
	$range =~ s/\s+//g;
	# die if invalid characters
	croak "invalid character passed in string [$range]!" 
			if $range =~ /[^\s,.\d]/;
	# not allowed a lone .
	croak "invalid range [$range] (single .)!" if $range =~ /[^.]+\.{1}[^.]+/;
	# not allowed more than 2 .
	croak "invalid range [$range] (more than 2 .)!" if $range =~ /[^.]+\.{3}/;
	
	@range = eval ($range);
	return @range;
}

</pre>


<a id="dayfourstep4"></a>
<h4>step 4) ...means more and more tests</h4> 

Now it is time to test this behaviour. Go edit <code>./t/01-validate.t</code> adding (append the following code to the end of the test file) some <code>dies_ok</code> statements preceded by a <code>note</code>:

<pre>
note ("start checks about incorrect dots in string");

dies_ok { Range::Validator::validate('1.2') }
			"expected to die with a lone dot";
			
dies_ok { Range::Validator::validate('0..2,5.6,8') }
			"expected to die with a lone dot";


</pre>
Run the test via <code>prove </code>

<pre>
shell> prove -l -v ./t/01-validate.t

./t/01-validate.t ..
ok 1 - use Range::Validator;
ok 2 - ok valid string produces correct number of elements
# starting test of forbidden characters in the string form
ok 3 - expected to die with invalid character
# start checks about incorrect dots in string
ok 4 - expected to die with a lone dot
ok 5 - expected to die with a lone dot
1..5
ok
All tests successful.
Files=1, Tests=5,  0 wallclock secs ( 0.06 usr +  0.03 sys =  0.09 CPU)
Result: PASS

</pre>
Fine! But.. to much repetitions in the test code. Are not we expected to be DRY (Dont Repeat Yourself)? Yes we are and since we have been so lazy to put <code>use Test::More qw(no_plan)</code> we can add a good loop of tests (replace the last two <code>dies_ok</code> with the following code in the test file):

<pre>
foreach my $string ( '1.2', '0..2,5.6,8', '1,2,.,3', '.' ){
	dies_ok { Range::Validator::validate( $string ) }
			"expected to die with a lone dot in range [$string]";
}

</pre>
Run the test again:

<pre>
shell> prove -l -v ./t/01-validate.t

./t/01-validate.t ..
ok 1 - use Range::Validator;
ok 2 - ok valid string produces correct number of elements
#   Failed test 'expected to die with a lone dot in range [.]'
# starting test of forbidden characters in the string form

#   at ./t/01-validate.t line 22.
ok 3 - expected to die with invalid character
# Looks like you failed 1 test of 7.
# start checks about incorrect dots in string
ok 4 - expected to die with a lone dot in range [1.2]
ok 5 - expected to die with a lone dot in range [0..2,5.6,8]
ok 6 - expected to die with a lone dot in range [1,2,.,3]
not ok 7 - expected to die with a lone dot in range [.]
1..7
Dubious, test returned 1 (wstat 256, 0x100)
Failed 1/7 subtests

Test Summary Report
-------------------
./t/01-validate.t (Wstat: 256 Tests: 7 Failed: 1)
  Failed test:  7
  Non-zero exit status: 1
Files=1, Tests=7,  0 wallclock secs ( 0.02 usr +  0.03 sys =  0.05 CPU)
Result: FAIL

</pre>
FAIL? Fortunately we shown the current range passed in the text generated by the test, so go examine it: 

<code>not ok 7 - expected to die with a lone dot in range [.]</code>

Spot why it fails (ie it does not die as expected)? Our regex to check a lone dot is:

<code>/[^.]+\.{1}[^.]+/</code>

And it reads (as per the <code>YAPE::Regex::Explain</code> output): any character except: '.' (1 or more times (matching the most amount possible)) followed by '.' (1 times) followed by any character except: '.' (1 or more times (matching the most amount possible)) 

Which is simply not true for the given string <code>'.'</code> So we try changing both plus signs with question mark quantifiers in the regex: it does not help. As a wise friend explains, we need lookaround: <code>/(?&lt;!\\.)\\.(?!\\.)/</code> will work! So we change the check in the module like follow: 

<pre>
# not allowed a lone .
	croak "invalid range [$range] (single .)!" if $range =~ /(?&lt;!\.)\.(?!\.)/; 

</pre>

As we spot this edge case we add two similar ones to the test:

<pre>
foreach my $string ( '1.2', '0..2,5.6,8', '1,2,.,3', '.', '1.', '.1' ){
	dies_ok { Range::Validator::validate( $string ) }
			"expected to die with a lone dot in range [$string]";
}

</pre>
Also the next regex (aimed to search for three dots) in the module is not working for the very same reason; change it from <code>/[^.]+\.{3}/</code> to simply <code>/\.{3}/</code>

The moral? Tests are your friends! We spot, by hazard, an edge case and our code must be able to deal with it, so free as much your fantasy writing your tests. Cockroaches come from box corners.. ops, no I mean: bugs come from edge case.

Now we add some test to spot, and die, if three dots are found, with the new simpler regex <code>/\.{3}/</code> so we change the code  adding the following code to the test:

<pre>
foreach my $newstring ( '1...3', '1,3...5','...', '1...', '...2' ){
	dies_ok { Range::Validator::validate( $newstring ) }
			"expected to die with three dots in range [$newstring]";
}
</pre>
We run the test:

<pre>
shell> prove -l -v ./t/01-validate.t

./t/01-validate.t ..
ok 1 - use Range::Validator;
ok 2 - ok valid string produces correct number of elements
# starting test of forbidden characters in the string form
ok 3 - expected to die with invalid character
# start checks about incorrect dots in string
ok 4 - expected to die with a lone dot in range [1.2]
ok 5 - expected to die with a lone dot in range [0..2,5.6,8]
ok 6 - expected to die with a lone dot in range [1,2,.,3]
ok 7 - expected to die with a lone dot in range [.]
ok 8 - expected to die with a lone dot in range [1.]
ok 9 - expected to die with a lone dot in range [.1]
ok 10 - expected to die with three dots in range [1...3]
ok 11 - expected to die with three dots in range [1,3...5]
ok 12 - expected to die with three dots in range [...]
ok 13 - expected to die with three dots in range [1...]
ok 14 - expected to die with three dots in range [...2]
1..14
ok
All tests successful.
Files=1, Tests=14,  1 wallclock secs ( 0.03 usr +  0.03 sys =  0.06 CPU)
Result: PASS

</pre>
So now your sub is:

<pre>
sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
	}
	# otherwise we received a list
	else{
		...
	}
	# remove any space from string
	$range =~ s/\s+//g;
	# die if invalid characters
	croak "invalid character passed in string [$range]!" 
			if $range =~ /[^\s,.\d]/;
	# not allowed a lone .
	croak "invalid range [$range] (single .)!" if $range =~ /(?&lt;!\.)\.(?!\.)/; 
	# not allowed more than 2 .
	croak "invalid range [$range] (more than 2 .)!" if $range =~ /\.{3}/;
	
	@range = eval ($range);
	return @range;
}

</pre>
And our test file <code>./t/01-validate.t</code> as follow:

<pre>
#!perl
use 5.006;
use strict;
use warnings;
use Test::More qw(no_plan);
use Test::Exception;

use_ok( 'Range::Validator' ); 

ok (scalar Range::Validator::validate('0..2') == 3, 
	'ok valid string produces correct number of elements' );

note ("starting test of forbidden characters in the string form");

dies_ok { Range::Validator::validate('xxxinvalidstringxxx') }
			"expected to die with invalid character";
			
note ("start checks about incorrect dots in string");

foreach my $string ( '1.2', '0..2,5.6,8', '1,2,.,3', '.', '1.', '.1' ){
	dies_ok { Range::Validator::validate( $string ) }
			"expected to die with a lone dot in range [$string]";
}

foreach my $newstring ( '1...3', '1,3...5','...', '1...', '...2' ){
	dies_ok { Range::Validator::validate( $newstring ) }
			"expected to die with three dots in range [$newstring]";
}

</pre>



<a id="dayfourstep5"></a>
<h4>step 5) git: a push for two commits</h4> 
Time to review the status of the local repository, commit changes and push it online:

<pre>
git-client> git status

On branch master
Changes not staged for commit:
  (use "git add &lt;file&gt;..." to update what will be committed)
  (use "git checkout -- &lt;file&gt;..." to discard changes in working directory)

        modified:   lib/Range/Validator.pm
        modified:   t/01-validate.t

no changes added to commit (use "git add" and/or "git commit -a")



git-client> git commit -a -m "changed regexes for 2 o lone dot and relative tests"

[master 169809c] changed regexes for 2 o lone dot and relative tests
 2 files changed, 17 insertions(+), 1 deletion(-)


 
git-client> git push YourGithubLogin master

fatal: HttpRequestException encountered.
   
Username for 'https://github.com': YourGithubLogin
Password for 'https://YourGithubLogin@github.com':
Counting objects: 12, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (12/12), 1.50 KiB | 385.00 KiB/s, done.
Total 12 (delta 5), reused 0 (delta 0)
remote: Resolving deltas: 100% (5/5), completed with 3 local objects.
To https://github.com/YourGithubLogin/Range-Validator
   5083ec3..169809c  master -> master

   
</pre>
Today we committed twice, do you remember? first time just the POD we added for the sub and second time just few moments ago.
We pushed just one time. What's really now in the online repository?

Go to the online repository, Insights, Network: the last two dots on the line segment are our two commits, pushed together in a single push. Handy, no? Click on the second-last dot and you will see the detail of the commit concerning the POD, with lines we removed in red and lines we added in green. Commits are free: committing small changes frequently is better than commit a lot of changes all together.





<a id="dayfive"></a>
<h2>day five: deeper tests</h2>


<a id="dayfivestep1"></a>
<h4>step 1) more validation in the code</h4>

Today we plan to add two new validations in our sub: first one intended to be used against ranges passed in string form, the second to all ranges, before returning them.

The constraint for the string form is about reversed ranges, like <code>3..1</code> and it is added just after the last <code>croak</code> we added yesterday:

<pre>
     # spot reverse ranges like 27..5
	 if ($range =~ /[^.]\.\.[^.]/){
		foreach my $match ( $range=~/(\d+\.\.\d+)/g ){
			$match=~/(\d+)\.\.(\d+)/;
			croak "$1 > $2 in range [$range]" if $1 > $2;
		}
	}

</pre>
Now is important that we take the habit to commit on our own, whenever we add an atomic piece of code: so go to commit! From now on not every git operation will be shown with full output, only important ones (is this a git guide? No!).

The other one, applied before returning the range as array, is about overlapping ranges: <code>(0..2,1)</code> that is equivalent to <code>0,1,1,2</code> with a nasty repetition terrible for the rest of the code outside the present module (this assumption is related to our current, fictional, scenario).
So, just before returning from the sub, we simply use a hash to have unique elements in the resulting array:

<pre>
	# eval the range
	@range = eval ($range);
	# remove duplicate elements using a hash
	my %single = map{ $_ => 1} @range;			# -- new line
	# sort unique keys numerically
	@range = sort{ $a &lt;=&gt; $b } keys %single;	# -- new line
	return @range;

</pre>
As previously said, commit on your own, with a meaningful comment.

You end with:

<pre>
sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
	}
	# otherwise we received a list
	else{
		...
	}
	# remove any space from string
	$range =~ s/\s+//g;
	# die if invalid characters
	croak "invalid character passed in string [$range]!" 
			if $range =~ /[^\s,.\d]/;
	# not allowed a lone .
	croak "invalid range [$range] (single .)!" if $range =~ /(?&lt;!\.)\.(?!\.)/; 
	# not allowed more than 2 .
	croak "invalid range [$range] (more than 2 .)!" if $range =~ /\.{3}/;
	# spot reverse ranges like 27..5
	if ($range =~ /[^.]\.\.[^.]/){
		foreach my $match ( $range=~/(\d+\.\.\d+)/g ){
			$match=~/(\d+)\.\.(\d+)/;
			croak "$1 > $2 in range [$range]" if $1 > $2;
		}
	}
	# eval the range
	@range = eval ($range);
	# remove duplicate elements using a hash
	my %single = map{ $_ => 1} @range;
	# sort unique keys numerically
	@range = sort{ $a &lt;=&gt; $b } keys %single;
	return @range;
}

</pre>
New features are worth to be pushed on the online repository: you know how can be done. Do it.




<a id="dayfivestep2"></a>
<h4> step 2) a git excursus</h4>

Did you follow my small advices about git committing and meaningful messages? If so it's time to see why is better to be diligent: with <code>git log</code> (which man page is probably longer than this guide..) you can review a lot about previous activities:

<pre>
git-client> git log HEAD --oneline

bb952ee (HEAD -> master, YourGithubLogin/master) removing duplicates from overlapping ranges
15a5f63 check for reverse ranges in string form
169809c changed regexes for 2 o lone dot and relative tests
a6dc557 initial POD to document validate function
5083ec3 added 01-validate.t
580f628 some code into validate, added 01-validate.t and modified Makefile.PL
49a0690 moved POD, removed -T
1788c12 module-starter created content

</pre>
This is definitevely handy. <code>HEAD</code> is where your activity is focused in this moment. Try to remove the <code>--oneline</code> switch to see also all users and dates of each commit.

As you can understand git is a vaste world: explore it to suit your needs. This is not a git guide ;)



<a id="dayfivestep3"></a>
<h4> step 3) add deeper tests</h4>

Until now we used a limited test arsenal: <code>ok</code> from <code>Test::Simple</code> <code>use_ok</code> and <code>note</code> from <code>Test::More</code> <code>dies_ok</code> from <code>Test::Exception</code>

As we added a <code>croak</code> in our sub to prevent reversed ranges, we can use <code>dies_ok</code> again to check such situations (append the following code to our test file):

<pre>
foreach my $reversed ('3..1,7..9','1..4,7..5','3..4, 7..5','0..2,27..5'){
	dies_ok { Range::Validator::validate( $reversed ) } "expected to die with reverse range [$reversed]";
}

</pre>
Commit at your will.

<code>Test::More</code> has a lot of useful testing facilities (review the module documentation to take inspiration) and now we will use <code>is_deeply</code> to implement some positive test about expected and returned data structures.

This is useful, in our case, to test that overlapping ranges or unordered ones are returned corrected. To do this we can use a hash of inputs and their expected returned values (append the following code to our test file):

<pre>
my %test = (
	'1,1..3'	=> [(1,2,3)],
	'1,2..5,4'	=> [(1,2,3,4,5)],
	'1..5,3'	=> [(1,2,3,4,5)],
	'8,9,1..2'	=> [(1,2,8,9)],
	'1..3,3,5..7'	=> [(1,2,3,5,6,7)],
	'5..7,1..6'		=> [(1,2,3,4,5,6,7)],
	'0..5,3'		=> [(0,1,2,3,4,5)]
);

# ranges, even if overlapped or unordered, return the correct array
foreach my $range ( keys %test ){
	my @res = Range::Validator::validate($range);
	is_deeply( $test{$range},\@res,
				"correct result for range [$range]"
	);
}

</pre>
Last two tests we added will produce the following output:

<pre>
ok 15 - expected to die with reverse range [3..1,7..9]
ok 16 - expected to die with reverse range [1..4,7..5]
ok 17 - expected to die with reverse range [3..4, 7..5]
ok 18 - expected to die with reverse range [0..2,27..5]
ok 19 - correct result for range [1,2..5,4]
ok 20 - correct result for range [1,1..3]
ok 21 - correct result for range [0..5,3]
ok 22 - correct result for range [5..7,1..6]
ok 23 - correct result for range [1..3,3,5..7]
ok 24 - correct result for range [8,9,1..2]
ok 25 - correct result for range [1..5,3]

</pre>
Commit.



<a id="dayfivestep4"></a>	
<h4> step 4) who is ahead? git branches and log </h4>

Just at glance: up to you to explore this topic. Look at the following git session of commands, two commands ( one that we never used until now) just before and reissued just after the push:



<pre>
git-client> git log HEAD --oneline

c3f8d5b (HEAD -> master) test for overlappped or unordered ranges
f16789a test for reversed ranges
bb952ee (YourGithubLogin/master) removing duplicates from overlapping ranges
15a5f63 check for reverse ranges in string form
169809c changed regexes for 2 o lone dot and relative tests
a6dc557 initial POD to document validate function
5083ec3 added 01-validate.t
580f628 some code into validate, added 01-validate.t and modified Makefile.PL
49a0690 moved POD, removed -T
1788c12 module-starter created content

git-client> git show-branch *master

* [master] test for overlappped or unordered ranges
 ! [refs/remotes/YourGithubLogin/master] removing duplicates from overlapping ranges
--
*  [master] test for overlappped or unordered ranges
*  [master^] test for reversed ranges
*+ [refs/remotes/YourGithubLogin/master] removing duplicates from overlapping ranges


git-client> git push YourGithubLogin master

fatal: HttpRequestException encountered.
   
Username for 'https://github.com': YourGithubLogin
Password for 'https://YourGithubLogin@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 1011 bytes | 505.00 KiB/s, done.
Total 8 (delta 6), reused 0 (delta 0)
remote: Resolving deltas: 100% (6/6), completed with 3 local objects.
To https://github.com/YourGithubLogin/Range-Validator
   bb952ee..c3f8d5b  master -> master
   
git-client> git log HEAD --oneline

c3f8d5b (HEAD -> master, YourGithubLogin/master) test for overlappped or unordered ranges
f16789a test for reversed ranges
bb952ee removing duplicates from overlapping ranges
15a5f63 check for reverse ranges in string form
169809c changed regexes for 2 o lone dot and relative tests
a6dc557 initial POD to document validate function
5083ec3 added 01-validate.t
580f628 some code into validate, added 01-validate.t and modified Makefile.PL
49a0690 moved POD, removed -T
1788c12 module-starter created content

git-client> git show-branch *master

* [master] test for overlappped or unordered ranges
 ! [refs/remotes/YourGithubLogin/master] test for overlappped or unordered ranges
--
*+ [master] test for overlappped or unordered ranges

</pre>




<a id="dayfivestep5"></a>
<h4> step 5) overall check and release</h4>

We just need some small change and our module will be ready for production. We left some part of our code behind and precisely the <code>else</code> part dedicated to incoming arrays:

<pre>
# otherwise we received a list
	else{
		...
	}
</pre>
and we can just fill it with <code>@range = @_;</code> and commit the change. 

But if the above is true, we have to move all string check inside the <code>if ( @_ == 1) {...</code> block! Do it and commit the change. Now our sub is like the following one:

<pre>
sub validate{
	my $range;
	my @range;
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		$range = $_[0];
		# remove any space from string
		$range =~ s/\s+//g;
		# die if invalid characters
		croak "invalid character passed in string [$range]!" 
				if $range =~ /[^\s,.\d]/;
		# not allowed a lone .
		croak "invalid range [$range] (single .)!" if $range =~ /(?&lt;!\.)\.(?!\.)/; 
		# not allowed more than 2 .
		croak "invalid range [$range] (more than 2 .)!" if $range =~ /\.{3}/;
		# spot reverse ranges like 27..5
		if ($range =~ /[^.]\.\.[^.]/){
			foreach my $match ( $range=~/(\d+\.\.\d+)/g ){
				$match=~/(\d+)\.\.(\d+)/;
				croak "$1 > $2 in range [$range]" if $1 > $2;
			}
		}
		# eval the range
		@range = eval ($range);
	}
	# otherwise we received a list
	else{
		@range = @_;
	}	
	# remove duplicate elements using a hash
	my %single = map{ $_ => 1} @range;
	# sort unique keys numerically
	@range = sort{ $a &lt;=&gt; $b } keys %single;
	return @range;
}

</pre>
Is our change safe? Well we have a test suit: <code>prove -l -v</code> will tell you if the change impacts the test suit (if tests are poor you can never be sure).

Now our module is ready for production. It just lacks of some good documentation. Not a big deal, but is our duty to document what the sub does effectively.

Add to the POD of our sub:

<pre>
Every string with occurences of a lone dot or more than two dots will be rejected causing an exception in the calling program.

Reverse ranges like in <code>'3..1'</code> passed as string will also cause an exception.

In both string and list form any duplicate element (overlapped range) will be silently removed. Any form of unordered list will be silently rerodered.

</pre>
Check git status and commit. Use <code>git log HEAD --oneline</code> to see that the local repository is three steps ahead of the remote one. Push the changes in the online repository. Use <code>git log HEAD --oneline</code> again to see what happened.




<a id="dayfivestep6"></a>
<h4>step 6) test list form</h4>

Even if it is simpler we have to test the array form of our sub. We can use this time an array of tests each element being another array with two elements: first the list we pass to the sub, then the list we expect back from the sub. Again using <code>is_deeply</code> is a good choice:

Add the following test to our file <code>01-validate.t</code>

<pre>
note ("starting test of list form");

my @test = (
	# passed  expected
	# correct ones
	[ [(0..3)], [(0,1,2,3)] ],
	[ [(0,1..3)], [(0,1,2,3)] ],
	[ [(0..3,5)], [(0,1,2,3,5)] ],
	# overlapped ones
	[ [(0..3,2)], [(0,1,2,3)] ],
	[ [(1,0..3)], [(0,1,2,3)] ],
	[ [(0..3,1..2)], [(0,1,2,3)] ],


);
foreach my $list ( @test ){
	my @res = Range::Validator::validate( @{$list->[0]} );
	is_deeply( \@{$list->[1]},\@res,
				"correct result for list: @{$list->[0]}"
	);
}

</pre>
Run the test: we reached the big number of 32 succesful test! Congratulations!

As always, commit the change with a meaningful comment and push this important set of changes to the online repository.




<a id="daysix"></a>
<h2>day six: testing STDERR</h2>


<a id="daysixstep1"></a>
<h4>step 1) the problem of empty lists</h4>

Our assumptions, in "day zero - the plan", were to accept only ordered, not overlapped lists or their string representations. Other software in the project (again: a fictional scenario), where our validation module is used, blindly pass what received from outside (many different sources) to our <code>validate</code> sub. With the output produced by our sub many other subs or methods are called. All these software (out of our control) assume that, if an empty list is received then ALL elements are processed. This seemed the right thing to do.
  
After the advent of our module some example usage can be:

<pre>
# all actions performed, no need to call our validate sub
actions_to_activate_account();

# only reset password and send mail with new password
my @valid_range = Range::Validator::validate(3,12);
actions_to_activate_account( @valid_range );

# or in the string form:
my $action_string = get_action_string_from_DB( actions => 'reset_pwd' );
# $action_string is '3,12'
my @valid_range = Range::Validator::validate( $action_string );
actions_to_activate_account( @valid_range );

# or in the array form:
my @actions = get_action_list_from_DB( actions => 'reset_pwd' );
# @actions is (3,12)
my @valid_range = Range::Validator::validate( @actions );
actions_to_activate_account( @valid_range );

</pre>
Right? The module goes in production and 98% of errors from the foreign part of the code base disappeared. Only 98%?
Yes.. 

Miss A of department Z call your boss in a berserk state: not all their errors are gone away. They use the list form but Miss A and the developer B are sure no empty lists are passed to your validate sub. You call the developer B, a good fellow, who explain you that list are generated from  a database field that cannot be empty (NOT NULL constraint in the database):

You - Listen B, if I emit a warning you'll be able to trap which list generated from the database provoked it?

B - Sure! Can you add this?

You - Yes, for sure. I can use a variable in Range::Validator namespace, let's name it <code>warnings</code> and you'll set it to a true value and only you, and not the rest of the company, will see errors on STDERR. Ok?

B - Fantastic! I'll add the variable as soon as you tell me.

You - Ok, but then I want to know which list provoked the error, right? For a coffee?

B - Yeah man, for a coffee, as always.







<a id="daysixstep2"></a>	
<h4>step 2) adding a Carp to the lake</h4>

So we add a line in the top of the module, just after VERSION: <code>our $WARNINGS = 0;</code> to let dev B to trigger our warnings. We commit even this small change.

Then we add to the sub a <code>carp</code> call triggered if <code>our $WARNINGS == 1;</code> and if <code>@_ == 0</code> and we add this as <code>elsif</code> condition:

<pre>
	# assume we have a string if we receive only one argument
	if ( @_ == 1){
		# STRING PART ...
	}
	elsif ( $WARNINGS == 1 and @_ == 0 ){
		carp "Empty list passed in! We assume all element will be processed.";
	}
	# otherwise we received a list
	else{
		# NON EMPTY LIST PART ...
	}	


</pre>
Git status, git commit on your own.





<a id="daysixstep3"></a>	
<h4>step 3) prepare the fishing road: add a dependency for our test</h4>

To grab <code>STDERR</code> in test we have to add a dependency to <code>Capture::Tiny</code> module which is able, with its method <code>capture</code> to catch  <code>STDOUT</code>  <code>STDERR</code> and  results emitted by an external command or a chunk of perl code. Handy and tiny module.

Do you remeber the place to specify a dependency? Bravo! Is in <code>Makefile.PL</code> and we did the same in "day three step 3" when we added two modules to the <code>BUILD_REQUIRES</code> hash. Now we add <code>Capture::Tiny</code> to this part (remeber to specify module name in a quoted string):

<pre>
BUILD_REQUIRES => {
        'Test::More' 		=> '0',
		'Test::Exception' 	=> '0',
		'Capture::Tiny'   	=> '0',		# -- new line
    },

</pre>
Commit this change.





<a id="daysixstep4"></a>	
<h4>step 4) go fishing the Carp in our test</h4>

Now in <code>01-validate.t</code> test file we first add the module with <code>use Capture::Tiny qw(capture)</code> and then, at the end we add some test of the warning behaviour:

<pre>
note ("test of warnings emitted");
{	
	local $Range::Validator::WARNINGS;
	
	my ($stdout, $stderr, @result) = capture { Range::Validator::validate() };
	unlike($stderr, qr/^Empty list passed in/, "no warning for empty list unless \$Range::Validator::WARNINGS");
	
	$Range::Validator::WARNINGS = 1;
	
	($stdout, $stderr, @result) = capture { Range::Validator::validate() };
	like( $stderr, qr/^Empty list passed in/, "right warning for empty list if \$Range::Validator::WARNINGS");	
	
}
</pre>
Run the test suit, commit this change. Use <code>git log HEAD --oneline</code> to visualize our progresses and push all recent commits to the online repository.

The new version goes in production. The good fellow calls you:

B - Ehy, we added your warnings..

You - And..?

B - We spotted our errors in the database.. 

You - And which kind of error?

B - Well.. do you know what perl sees when it spot 1, followed by FOUR dots, followed by 3?

You - Ahh aha ah ah.. unbelievable! Yes, I suppose it parses as: from 1 to .3 aka nothing, aka empty list..

B - Exactly! Can you imagine my boss face?

You - I dont want! A coffee is waiting  for you. Thanks!




<a id="daysixstep5"></a>
<h4>step 5) document the new warning feature</h4>

Add some POD,few lines are better than nothing, to the module documentation:

<pre>
=head1 ENABLE WARNINGS

If the <code>$Range::Validator::WARNINGS</code> is set to a true value then an empty list passed to <code>validate</code> will provoke a warning from the caller perspective.

</pre>
Commit this change and update the online repository.





<a id="dayseven"></a>
<h2>day seven: the module is done but not ready</h2>


<a id="daysevenstep1"></a>
<h4>step 1) sharing</h4>

As stated in "day zero - the plan" sharing early is a good principle: can be worth to ask in a forum dedicated to Perl (like <a href="https://perlmonks.org">perlmonks.org</a>) posting a RFC post (Request For Comments) or using  the dedicated website <a href="http://prepan.org/">http://prepan.org/</a> to collect suggestions about your module idea and implementation. 



<a id="daysevenstep2"></a>	
<h4>step 2) files in a CPAN distribution</h4>

Your module is ready to be used and it is already used, but is not installable by a CPAN client nor can be indexed by a CPAN indexer at the moment. Read the short but complete description of possible files at <a href="https://www.perlmonks.org/index.pl?node_id=1009586">What are the files in a CPAN distribution?</a>

Following tests are not needed to install or use your module but to help you spotting what can be wrong in your distribution.





<a id="daysevenstep3"></a>	
<h4>step 3) another kind of test: MANIFEST</h4>


In the the "day one - preparing the ground" we used <code>module-starter</code> to create the base of our module. Under the <code>/t</code> folder the program put three test we did not seen until now: <code>manifest.t</code> <code>pod-coverage.t</code> and <code>pod.t</code>  

These three tests are here for us and they will help us to check our module distribution is complete. Let's start from the first

<pre>
shell> prove ./t/manifest.t

./t/manifest.t .. skipped: Author tests not required for installation
Files=1, Tests=0,  0 wallclock secs ( 0.03 usr +  0.01 sys =  0.05 CPU)
Result: NOTESTS

</pre>
Ok, no test run, just skipped. Go to view what is inside the test: it skips all actions unless <code>RELEASE_TESTING</code> environment variable is set. It also will complain unless a minimal version of <code>Test::CheckManifest</code> is installed. So set this variable in the shell (how to do this depends on your operating system: linux users probably need <code>export RELEASE_TESTING=1</code> while windows ones will use <code>set  RELEASE_TESTING=1</code>) and use your CPAN client to install the required module (normally <code>cpan Test::CheckManifest</code> is all you need) and rerun the test again:

<pre>
shell> prove ./t/manifest.t

./t/manifest.t ..
#   Failed test at ./t/manifest.t line 15.
./t/manifest.t .. 1/1 #          got: 0
#     expected: 1
# The following files are not named in the MANIFEST file:  .... # MANY LINES MORE..

</pre>
Omg?! What is all that output? The test complains about a lot of files that are present in the filesystem, in our module folder but are not specified in the <code>MANIFEST</code> file. This file contains a list (one per line) of files contained within the tarball of your module.

In the above output we have seen a lot, if not all, files under the <code>.git</code> directory. Obviously we do not want them included in our module distribution. How can we skip them? Using <code>MANIFEST.SKIP</code> file that basically contains regular expressions describing which files should be excluded from the distribution.

So go create this file in the main folder of the module and add inside it a line with a regex saying we do not want the <code>.git</code> directory:
<code>^\.git\/</code> and add this file with <code>git add MANIFEST.SKIP</code> and commit this important change.

Rerun the test (added some newlines for readability):

<pre>
shell> prove ./t/manifest.t

./t/manifest.t .. 1/1
#   Failed test at ./t/manifest.t line 15.
#          got: 0
#     expected: 1
# The following files are not named in the MANIFEST file: 

/path/to/your/module/ignore.txt, 
/path/to/your/module/MANIFEST.SKIP, 
/path/to/your/module/t/01-validate.t, 
/path/to/your/module/xt/boilerplate.t

...
</pre>
By far better: the test points us to two files we for sure need to include in <code>MANIFEST</code> and precisely: <code>MANIFEST.SKIP</code> and <code>t/01-validate.t</code>

Go to the <code>MANIFEST</code> file and add them (where they are appropriate, near similar files and paying attention to case an paths), then commit the change. If you rerun the above test you'll see files added to <code>MANIFEST</code> are no more present in the failure output.

Let's examine the remaining two files. What is <code>ignore.txt</code>? It was created as default ignore list by <code>module-starter</code> and it contains many lines of regexes. If we want <code>module-starter</code> to create <code>MANIFEST.SKIP</code> instead, next time we'll use it specify <code>--ignores='manifest'</code> For the moment we can delete it. Commit.

If you rerun the test you now see only <code>/xt/boilerplate.t</code> and, if you open it, you'll see that is just checking if you left some default text in our module, texts put by <code>module-starter</code> Ah! useful test: let's run it:

<pre>
shell> prove ./xt/boilerplate.t

./xt/boilerplate.t .. ok
All tests successful.

Test Summary Report
-------------------
./xt/boilerplate.t (Wstat: 0 Tests: 3 Failed: 0)
  TODO passed:   3
Files=1, Tests=3,  1 wallclock secs ( 0.03 usr +  0.03 sys =  0.06 CPU)
Result: PASS

</pre>
Ok no boilerplate garbage left. We can delete this test file and commit the change.

Now, finally:

<pre>
shell> prove ./t/manifest.t

./t/manifest.t .. ok
All tests successful.
Files=1, Tests=1,  1 wallclock secs ( 0.02 usr +  0.03 sys =  0.05 CPU)
Result: PASS

</pre>
Push recent changes into the online repository.




<a id="daysevenstep4"></a>
<h4>step 4) another kind of test: POD and POD coverage</h4>

In our <code>/t</code> folder we still have two tests we did not run: shame! <code>module-starter</code> created for us <code>pod.t</code> and <code>pod-coverage.t</code> The first one checks every POD in our distribution has no errors and the second ensures that all relevant files in your distribution are appropriately documented in POD documentation. Thanks for this. Run them:

<pre>
shell> prove -l -v ./t/pod.t

./t/pod.t ..
1..1
ok 1 - POD test for lib/Range/Validator.pm
ok
All tests successful.
Files=1, Tests=1,  0 wallclock secs ( 0.03 usr +  0.02 sys =  0.05 CPU)
Result: PASS


shell> prove -l -v ./t/pod-coverage.t

./t/pod-coverage.t ..
1..1
ok 1 - Pod coverage on Range::Validator
ok
All tests successful.
Files=1, Tests=1,  0 wallclock secs ( 0.03 usr +  0.02 sys =  0.05 CPU)
Result: PASS

</pre>




	
<a id="daysevenstep5"></a>
<h4>step 5) some README and final review of the work</h4>

The <code>README</code> must contain some general information about the module. Users can read this file via <code>cpan</code> client so put a minimal description in it. Gihub website use it as default page, so it is useful have some meningful text. Someone generates the text from the POD section of the module. Put a short description, maybe the sysnopsis and commit the change. Push it online.

Now we can proudly look at our commits history in a <code>--reverse</code> order:

<pre>
git-client> git log HEAD --oneline --reverse

1788c12 module-starter created content
49a0690 moved POD, removed -T
580f628 some code into validate, added 01-validate.t and modified Makefile.PL
5083ec3 added 01-validate.t
a6dc557 initial POD to document validate function
169809c changed regexes for 2 o lone dot and relative tests
15a5f63 check for reverse ranges in string form
bb952ee removing duplicates from overlapping ranges
f16789a test for reversed ranges
c3f8d5b test for overlappped or unordered ranges
89174fe in the else block @range = @_
58dbb12 moved string checks into the if (@_ == 1) block
8697b87 added POD for all string and list cecks
e4f8eb1 added tests for lists
3efd7ce added $WARNING = 0
a46d6fc elsif block to catch empty @_ and carping under request
3e5993d Capture::Tiny in Makefile.pl
ac22e82 test for warnings emitted
9667e22 POD for warnings
13f53eb MANIFEST.SKIP first line
99ab999 MANIFEST added MANIFEST.SKIP and 01-validate.t
61b7c9f removed ignore.txt
e3feb61 removed xt/boilerplate.t
3c0da4f (HEAD -> master, YourGithubLogin/master) modified README

</pre>
A good glance of two dozens of commits! We have done a good job, even if with some errors: committing multiple changes in different part of the project (like in our third commit) is not wise: better atomical commits. We have also some typo in commit messages.. 






<a id="daysevenstep6"></a>
<h4>step 6) try a real CPAN client installation</h4>

It's now time to see if our module can be installaed by a cpan client. Nothing easier: if you are in the module folder just run <code>cpan .</code> and enjoy the output (note that this command will modify the content of the directory!).





<a id="dayeight"></a>
<h2>day eight: other module techniques</h2>

<a id="dayeightoptionone"></a>
<h4>option one - the bare bone module</h4>

This is option we choosed for the above example and, even if it is the less favorable one, we used this form for the extreme easy. The module is just a container of subs and all subs are available in the program tha uses our module but only using their fully qualified name, ie including the name space where they are defined: <code>Range::Validator::validate</code> was the syntax we used all over the tutorial.

Nothing bad if the above behaviour is all you need.




<a id="dayeightoptiontwo"></a>
<h4>option two - the Exporter module</h4>

If you need more control over what to be available to the end user of your module <code>Exporter</code> CORE module will be a better approach.

Go read the module <a href="http://perldoc.perl.org/Exporter.html">documentation</a> to have an idea of its usage.

You can leverage what to export into the program using your module, so no more fully qualified package name will be needed. I suggest you to no export nothing by default (ie leaving <code>@EXPORT</code> empty) using instead <code>@EXPORT_OK</code> to let the end user to import sub from your module on, explicit, request.

With the use of <code>Exporter</code> you can also export variables into the program using your module, not only subs. It's up to you to decide if this is the right thing to do. Pay attention with names you use and the risk of name collision: what will happen if two module export two function with the same name? 

Perl is not restrictive in any meaning of the word: nothing will prevent the end user of your module to call <code>Your::Module::not_exported_at_all_sub()</code> and access its functionality. A fully qualified name will be always available. The end user is breaking the API you provide, API where <code>not_exported_at_all_sub</code> is not even mentioned. 


	
<a id="dayeightoptionthree"></a>
<h4>option three - the OO module</h4>

Preferred by many is the Object Oriented (OO) way. OO it's not better nor worst: it's a matter of aptitude or a matter of needs. See the relevant section on the core documentation: <a href="http://perldoc.perl.org/perlmodstyle.html#To-OO-or-not-to-OO%3f ">To-OO-or-not-OO?</a> about the choice.

An object is just a little data structure that knows the class (the package) it belongs to. Nothing more complex than this. The data structure is generally a hash and its consciouness of its class (package) is provided by the <code>bless</code> core function.

Your API will just provide a constructor (conventionally <code>new</code>) and a serie of methods this object can use.

Again: nothing prevents end user to call one of your function by its fully qualified name as in <code>Your::Module::_not_exported_at_all_sub()</code>
 it's just matter of being polite.
 
The core documentation include some tutorial about objects:

<a href="http://perldoc.perl.org/perlobj.html">perlobj</a>

<a href="http://perldoc.perl.org/perlootut.html">perlootut</a>

Many perl authors nowadays use specialized modules to build up OO projects: <code>Moose</code> module or the lighter flavor one <code>Moo</code> notably.

An OO module has many advantages in particular situations but is generally a bit slower than other module techniques.



	
<a id="dayeightadvancedMakefile.PLusage"></a>
<h4>advanced Makefile.PL usage</h4>

Until now we modified the <code>BUILD_REQUIRES</code> to specify dependencies needed while testing our module and <code>PREREQ_PM</code> to include modules needed by our module to effectively run.

The file format is described in the documentation of <code>ExtUtils::MakeMaker</code>  where is stated that, since version 6.64 it is available another field: <code><code>TEST_REQUIRES</code></code> defined as: "A hash of modules that are needed to test your module but not run or build it". This is exactly what we need, but this force us to specify, also in <code>Makefile.PL</code> that we need <code>'ExtUtils::MakeMaker'  => '6.64'</code> in the <code>CONFIGURE_REQUIRES</code> hash. 

The 6.64 version of <code>ExtUtils::MakeMaker</code> was released in 2012 but you cannot be sure end users have some modern perl, so we can safely use <code>BUILD_REQUIRES</code> as always or use some logic to fallback to "older" functionality if <code>ExtUtils::MakeMaker</code> is too old. You can use <code>WriteMakefile1</code> sub used in the <code>Makefile.PL</code> of  <code>App::EUMM::Upgrade</code>

<a id="dayeightothertestingmodules"></a>
<h4>other testing modules</h4>

In the current tutorial we used <code>Test::Exception</code> to test failures: consider also <code>Test::Fatal</code>

Overkill for simple test case but useful for complex one is the module  <a href="https://metacpan.org/pod/Test::Class">Test::Class</a>

Other modules worth to see are in the <a href="https://metacpan.org/pod/Task::Kensho#Task::Kensho::Testing:-Testing">Task::Kensho</a> list.

	
<a id="dayeightadvancedtestingcode"></a>
<h4>advanced testing code</h4>

If in your tests you have the risk of code repetition (against the DRY - Dont Repeat Yourself principle) you can find handy to have a module only used in your tests, a module under the <code>/t</code> folder. 

You need some precautions, though. 

Let's assume you plan a test helper module named  <code>testhelper</code> contained in the <code>/t/testhelper.pm</code> file used by many of your test files. 

You dont want CPAN to index your <code>testhelper</code> module and, to do so, you can put a <code>no_index</code> directive into your main <code>META.yml</code> or <code>META.json</code> file (or both). You can also use a trick in your package definition inserting a newline between <code>package</code> declaration and the name of the package. Like in:

<pre>
package		# hide from CPAN indexer
	testhelper; 

</pre>

In all tests you want to use that helper module you must:

<pre>
use lib '.';
use t::testhelper;

</pre>

<a id="bibliography"></a>
<h2>bibliography</h2>

<a id="COREdocumentationaboutmodules"></a>
<h4>CORE documentation about modules</h4>


<ul>
	<li>
		https://perldoc.perl.org/perlmod.html
	</li>
	<li>
		https://perldoc.perl.org/perlnewmod.html
	</li>
	<li>
		 https://perldoc.perl.org/perlmodstyle.html
	</li>
	<li>
		 http://perldoc.perl.org/perlobj.html
	</li>
	<li>
		 http://perldoc.perl.org/perlootut.html
	</li>
</ul>



<a id="COREdocumentationabouttesting"></a>
<h4>CORE documentation about testing</h4>

<ul>
	<li>
		https://perldoc.perl.org/Test.html
	</li>
	<li>
		https://perldoc.perl.org/Test/Simple.html
	</li>
	<li>
		 https://perldoc.perl.org/Test/More.html
	</li>
	<li>
		 https://perldoc.perl.org/prove.html
	</li>
	<li>
		 other CORE modules under the Test:: namespace
	</li>
	<li>
		 modules under the TAP:: namespace
	</li>
</ul>




<a id="furtherreadingsaboutmodules"></a>	
<h4>further readings about modules</h4>

<ul>
	<li>
		https://www.perlmonks.org/index.pl?node_id=102347 - Simple Module Tutorial
	</li>
	<li>
		https://www.perlmonks.org/index.pl?node_id=431702  - José's Guide for creating Perl modules
	</li>
	<li>
		 https://www.perlmonks.org/index.pl?node_id=418891  - Writing Solid CPAN Modules 
	</li>
	<li>
		 https://www.perlmonks.org/index.pl?node_id=553487  - On Interfaces and APIs
	</li>
	<li>
		 https://www.perlmonks.org/index.pl?node_id=158999  - How to make a CPAN Module Distribution
	</li>
	<li>
		 https://www.perlmonks.org/index.pl?node_id=1009586 - What are the files in a CPAN distribution?
	</li>
	<li>
		 http://tynovsky.github.io/cpan-tutorials/ 
	</li>
	<li>
		 http://modernperlbooks.com/books/modern_perl_2016/07-object-oriented-perl.html
	</li>
	<li>
		https://metacpan.org/pod/Module%3A%3AStarter
	</li>
</ul>


<a id="furtherreadingsabouttesting"></a>
<h4>further readings about testing</h4>
<ul>
	<li>
		 http://modernperlbooks.com/books/modern_perl_2016/09-managing-real-programs.html
	</li>
	<li>
		 http://shop.oreilly.com/product/9780596100926.do
	</li>
	<li>
		 https://qa.perl.org/testing/
	</li>
	<li>
		 http://petdance.com/perl/automated-testing/
	</li>
	<li>
		 https://www.perlmonks.org/index.pl?node_id=1195817 - Test Driven Development, for software and for pancakes
	</li>
</ul>


<a id="acknowledgements"></a>
<h2>acknowledgements</h2>

As all my works the present tutorial would be not possible without the help of the perlmonks.org community.
Not being an exhaustive list I want to thanks: Corion, choroba, Tux, 1nickt, marto, hippo, haukex, Eily, eyepopslikeamosquito, davido and kschwab (to be updated ;)

</body>
</html>

