---
layout:   default
title:    Speakers - GoRuCo 2010
author:   Jesse
template: speakers
---

Speakers
=====

<a name="dix"></a>

## [Paul Dix](http://pauldix.net/) Building Web Service Clients with ActiveModel

With the introduction of ActiveModel, Rails is no longer bound by a
specific ORM (ActiveRecord). ActiveModel exposes not only a common
interface for the Rails 3 model layer, but also a set of tools for
building data models. This talk will go over techniques and code for
using web services as a model layer with clients that leverage
ActiveModel's functionality.

This talk will cover how to use ActiveModel to write web service
client libraries that can be used as a drop in replacement for
ActiveRecord based models. This means they will work in form view
helpers and with Rails' routes and url generation. The primary topics
will cover validation, serialization, request logic, use in
development, and compliance testing.

The list of topics and technologies covered will include:
How to write client side validations with ActiveModel::Validations.
How to write clear libraries that use ActiveModel::Serializers.
How to abstract connection logic and ensure parallel execution and
speed (using Typhoeus or a threaded model).
How to test your library's compliance with ActiveModel::Lint coverage.

While there has been some coverage of ActiveModel already in some blog
posts, this talk will dive deeper and show how it can be used
specifically for writing easy to use, readable, maintainable, and
performant web service client libraries.

Attendees should be familiar with Ruby and Rails. Knowledge about
asynchronous and threaded programming is helpful, but not required.

Paul Dix is the author of the book "Service Oriented Design with Ruby
and Rails". He is a founder and the CTO at Market.io. In the past he
has worked at Google, Microsoft, McAffee, Air Force Space Command, and
various startups filling positions as a programmer, software tester,
and network engineer. Paul is the author of the open source Ruby
libraries SAXMachine, Feedzirra, and Typhoeus. He has a degree in
computer science from Columbia University.


<a name="gauthier"></a>

## [Nick Gauthier](http://www.smartlogicsolutions.com/nick) Grease your Suite: Tips and Tricks for Faster Testing

<!--
<div class="headshot">
<img src="/images/greg_brown.png">
</div>
-->

Continuous integration is a great way to keep your code base organized and well tested. But when a test suite takes so long to run that developers stop running it before every commit, they lose their constant feedback loop and quality drops. In this talk we'll explore methods of speeding up the test suite so that developers can be confident about the code they've written before they share it with the team.

We'll start with quick cheap fixes, like optimizing your operating system, that can yield drastic results (like cutting test time in half!) with no loss of functionality. We'll also cover methods of writing tests that reduce their run time with gems like fast\_context for shoulda. At then end, we'll move to more involved methods of multi-tasking your test suite to run on all the cores in your workstation and even to setting up a distributed testing cloud to run all your tests in parallel.

Every tactic will be backed up with hard benchmarks from real production code. We'll show the evolution of a test suite from its full run time of 13 minutes down to a number you won't believe. By the end of the presentation, attendees will have learned methods that they can apply to their own projects to help speed up their development process.

Attendees should be familiar with testing a rails project. Knowledge of linux/unix is a plus, and knowing shoulda will make the test code easier to read.

Nick Gauthier is a developer and technical lead at [SmartLogic Solutions](http://www.smartlogicsolutions.com/nick), a Baltimore web development company. He's been using linux on the desktop for almost a decade now, and started coding rails two years ago. He's an active attendee and occasional speaker at Bmore on Rails. He's developed a number of performance-obsessed ruby gems, like slow-actions, multitest, and hydra.

<a name="golick"></a>

## [James Golick](http://jamesgolick.com/) Scaling to Hundreds of Millions of Requests: What Worked and What Didn't

All over the web, people are discussing the latest scalable database, the newest testing strategy, or even cloud computing. Claims are made about scalability, reliability, and performance. But by definition, most of this hype is simply conjecture. Its authors rarely have the experience to support their claims.

In the process of scaling our ruby, rails, and scala app to 150 million monthly pageviews, we've tested a lot of these technologies and ideas. We've put several popular and supposedly scalable NoSQL database solutions in to heavy production use. We've tried testing frameworks and ideas. We've deployed both cloud computing instances and physical hardware. Some things worked - others failed spectacularly.

In this talk, I'll share our experiences, good and bad. These are some of the topics we'll cover:

* Virtualization and Cloud Computing: Virtualized hardware is the default choice for new ruby deployments. That makes sense - it's easy to get started, and you only pay for what you need. But when (if ever) does it make sense to move to physical hardware? It might be sooner than you think.
* NoSQL: NoSQL is all the rage in the ruby community. There are quite a few solutions, nearly all of them advertised as fast, scalable, reliable. But what is it really like to run and maintain them in production?
* Rails Best-Practices: There are certain practices rails developers take for granted. Automated testing and fat models are a given on almost every rails project. But are these really optimal strategies? Are there ways we can write better-designed, more maintainable code?

James spends his days (and most of his nights) scaling and maintaining a high traffic rails app. In the process, he hacks on ruby libraries like friendly and cassandra\_object, writes scala code, and manages a growing array of servers. James is obsessive about refining his craft. He reads and writes about design patterns, SOLID, and mockist testing. James is currently CTO of Protose Inc.

<a name="gupta"></a>

## [Aman Gupta](http://github.com/tmm1) memprof: the ruby level memory profiler

Ever wondered why your ruby script uses so much RAM? Tired of having
god restart your rails app every few hours?

This talk will introduce memprof, a ruby level memory profiler. We'll
demo memprof on a variety of real-world examples, including some
popular open source projects, to find and fix memory leaks. Along the
way, we'll learn how the ruby VM manages memory, why garbage
collection has such a large impact on ruby's performance and some
common ways to reduce the memory usage of your ruby applications.

Aman is a serial entrepreneur, ruby hacker and a recent winner of a
Ruby Heroes award. He currently maintains the EventMachine project and
various other gems that help build high-performance distributed and
asynchronous systems in ruby, including em-mysql, em-spec, jsSocket
and amqp.

Most recently, Aman has been hacking on performance improvements to
MRI, and tools for the VM such as perftools.rb, a sampling profiler
for ruby code based on google-perftools, and gdb.rb, a MRI specific
version of gdb.

<a name="maccaw"></a>

## [Alex MacCaw](http://www.eribium.org/) Bowline - Ruby Desktop Applications

If you've ever wished creating desktop application was as easy as creating a Rails site, then this session is for you. Developed in a real business environment, Bowline is a Ruby desktop framework that is aiming to be the Rails of the desktop world.

Bowline's author will take you through creating beautiful interfaces in HTML5, CSS3 and JavaScript; then binding those interfaces to the Ruby backend - producing a fully featured cross-platform desktop application.

Bowline uses WebKit for it's interface, so all the new CSS3 and HTML5 developments are available to you. The session will show you how to use all these new tools in Bowline apps, from CSS animations to completely new layout techniques.

The session will then conclude by showing you how to synchronize Bowline apps with your remote servers Ð building fully realtime desktop applications.

Alex is a Ruby developer and entrepreneur from London. His first open source project, Juggernaut, was released 3 years ago. Since then, Alex has been working on numerous other projects - the latest of which, Bowline was developed for his company's latest product, Taskforce. He writes for a widely followed blog, and has contributed to many others - including the Rails Magazine. He's also spoken at quite a few events, such as Rails Conf Europe last year.

<a name="melia"></a>

## [Luke Melia](http://www.lukemelia.com/) Managing Ruby Teams

Why a talk on managing a development team at a Ruby conference? That would imply that managing a team of Ruby developers is different than managing other development teams. Not just different as in Ruby-is-more-dynamic-and-expressive-than-Java different... although language properties do influence team dynamics and collaboration styles. Not just different as in the fast-changing, entrepreneurial types of environment that Ruby tends to be deployed in... though those environments certainly present challenges to leading and motivating teams.

The key difference is managing Ruby developers is... Ruby developers. Generalizing, Ruby developers are a self-selected group of independent thinkers. Developers who view their work as a craft and take tremendous pride what they build. Ruby developers are community-minded. Ruby developers are early adopters.

Technology management leaders tend to underestimate these differences. And that's a shame, because having a good manager is a key factor in job satisfaction, and the success of projects and teams.

This talk will cover the philosophy and techniques that I've used in managing Ruby teams over the last 3 years at Oxygen and Weplay.

Luke Melia is VP, Engineering at Weplay and was Director of Software Development at Oxygen Media until it was sold to NBC. Prior to that, he owned a small software company in Charlottesville, Virginia. Since discovering Ruby in 2005, he has has been active in the Ruby community, helping to organize the first GoRuCo,  presenting at nyc.rb, contributing to several open source projects including Tracks and Rails, and contributing a chapter to the lsat year's "Ruby in Practice", from Manning. He loves beach volleyball and lives in Chelsea with his wife and two daughters.

<a name="williams"></a>

## [Chris Williams](http://www.iterativedesigns.com) Rails' Best Caching Method is JavaScript

One of the most critical and often overlooked (and abused) elements of any web application is the JavaScript component. In the Rails world, there is a constant and expensive circle of instrumenting, optimizing, and scaling, which can quickly wear down a team and seed funding. This talk dives deep into super JavaScript nerdery to massively "rethink" the way a Rails application is designed and put into production. I have implemented and deployed this for a variety of sites when Rails performance and scaling became overly complex and expensive. With just a (beautiful) few lines of JavaScript, scale and performance became a non-issue. Furthermore this technique also facilitates moving "high traffic" components into better and faster implements with limited effort.

Chris Williams is the curator of JSConf, owner of Iterative Designs, and VP of OurParents. More commonly known, internetwise, by the handle of voodootikigod,  he has been known from time to time to fancy a good beer. With a Masters Degree in Computer Science from Virginia Tech, he has been a network security developer for the DOD, Security Engineer for TSA, and a parallel entrepreneur. In terms of Ruby, I have whole slew of Ruby/Sinatra/Rails/etc projects from a directory service, legal office groupware, automated patent aggregation and analysis tools, and a full stack call center system. 

