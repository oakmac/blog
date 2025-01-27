---
title: 'Clojure Text Editors'
datePublished: '2019-11-30'
dateModified: '2020-05-26'
slug: clojure-text-editors
summary: Focus on learning and writing Clojure!
author: 'Thomas Mattacchione'
---

<aside class="blog-content__note">Interested in jumping right to my editor setup? <a class="blog-content__link" href="#my-text-editor-setup">click here</a> or you can checkout my free <a class="blog-content__link" target="_blank" rel="noopener noreferrer" href="https://www.youtube.com/playlist?list=PLaGDS2KB3-AqeOryQptgApJ6M7mfoFXIp">Atom Setup Guide Video Series</a>.</aside>

Becoming a great software developer probably has more to do with ones ability to accept opportunities to revisit and refine _opinions_ and _beliefs_ than we would initially think.

In order to get to a point where this is possible, my strategy is usually to be "new" at something again.  For example, learn a **different** programming language.

Clojure is great for this because it gives you a break from common paradigms and exposes you to [functional programming](https://www.geeksforgeeks.org/functional-programming-paradigm/) and this sexy moon man language called [lisp](https://en.wikipedia.org/wiki/Lisp_(programming_language)).

So now that I was at a point where I was ready to learn Clojure I needed to use a "Clojure Editor".  I wanted to do this because I wanted to [think](https://www.youtube.com/watch?v=f84n5oFoZBc) as a Clojurist and use the same tools as them. This meant [emacs](https://www.gnu.org/software/emacs/) because all my research and conversations up until this point with other Clojurists led me to the opinion that `emacs` was _the_ "Clojure Editor".

<aside class="blog-content__note">Take note of the line <code class="gatsby-code-text">conversations up until this point with other Clojurists</code>.  While "use emacs" is how I interpreted what they were saying, and some even used those words, it was not actually what they were saying.  By the end of this post I will hopefully transcribe the real message as I now understand it.</aside>

Turns out that choosing emacs was not a great choice for me.  I should have stuck with the editor I knew best so that I could focus on being new at one thing at a time.  More on that later.

All of this is to say, here is an article that outlines the landscape of Clojure Editors which will hopefully help to inform your initial steps into Clojure land.

The rest of this article will be [bikeshed](https://www.urbandictionary.com/define.php?term=bikeshed) city. The hope? By documenting the thoughts and providing a few words of encouragement we can save some future Clojure developer some time.

<aside class="blog-content__note">Text Editors are a source of furious debate among programmers.  So if the opinions expressed herein enrage, please know that is not my intention.  I love you.  For those who just want to see how I setup my Text Editor for Clojure development, jump to the <a href="#my-text-editor-setup">third section</a> of this post.  Also note that my recommendations are for both Clojure and ClojureScript.</aside>

## Clojure Text Editors

Let's start by introducing the top Text Editors for Clojure(Script) development based on the 2020 Clojure Survey Results<a href="#popular-editors" aria-describedby="footnote-label" id="popular-editors-ref">:</a>

1. [Emacs](https://www.gnu.org/software/emacs/)
1. [IntelliJ](https://www.jetbrains.com/idea/)
1. [VS code](https://code.visualstudio.com/)
1. [Vim](https://www.vim.org/)
1. [Atom](https://atom.io/)
1. [Sublime](https://www.sublimetext.com/)
1. [Eclipse](https://www.eclipse.org/downloads/)
1. [Light Table](http://lighttable.com/)

For professional and hobby developers, the above list contains the editors you might expect to see.  The issue is that for newcomers and developers without a strong idea of language specific tooling the above list can feel prohibitive.

One reason for this feeling is that since the majority of the Clojure developers are using the first 3, those must be the ones to use in order to be productive with Clojure.

If you feel this way and don't read any further please take this with you:  You **DO NOT** need to use Emacs or IntelliJ to learn or become excellent at Clojure.

This leads to the next part:  which editor should you use?

## Which Text Editor to Use

To figure out which editor to use for Clojure development try to answer the following question.  Are you:

- **A**. Experience developer (serious hobbyist or professional)
- **B**. New(ish) to programming

If you chose **A.** stick with the editor your currently using.  If you chose **B.** try `Atom` or `VS Code`.  Continue reading to find out why!

A Text Editor is one of a developer's primary tools because we spend most of our work life inside of it.  Given the time we spend in our Text Editor there is something to be said for the satisfaction we derive from using it and its impact on our productivity.

Over time, this satisfaction grows and we begin to associate the qualities of the developer with the editor itself.  It becomes a [zero sum game](https://www.merriam-webster.com/dictionary/zero-sum%20game).

There are some problems with this mentality and it begins with the fact that tools are tools.  They either facilitate productivity, or they don't.  Further, the productivity one human gains from a tool, the satisfaction as we called it earlier, is likely going to be different from the next person.  You do you.

Knowing this, here's how I define productivity: low `startup cost` + the `utility` of the editor itself.  Here's what I mean by this:

`Startup cost` is about whether or not I can use the editor regardless of my operating system and how much configuration I need to get it going on a new development environment.

`Utlity` is performance and customizability of the Editor.  For performance, what I mean is that when I do things like search, open large files or use plugins that are supposed to make me more productive, but I have to literally stop what I am doing and wait for the editor sort itself out, this is no bueno.

Then there is customization.  This is a worthwhile optimization which, to me, means I can add features to the editor to improve my workflow.  It also helps when I can do this with languages and tool chains I already know.

All of this is to say that these are my preferences that I have built through years of experimentation.  If you have been developing for a while, you will have likely gone through a similar process.  But let's go back to the original question of "which text editor to choose?".

As I said earlier, if you're an experienced developer, go with the editor you know.  If you are a new programmer and don't have deep ties to any particular editor, choose `Atom` or `VS Code`.  The reason for this recommendation is because these editors are easy to use, work on all operating systems, have active and easy to access communities and support all the modern Clojure tooling one could ever want.

Im comparison, if you choose an editor like Emacs, Vim, or Intellij you are going to spend more time learning and configuring the editors than learning Clojure.  You can always try these editors when you feel more accomplished with Clojure and want to optimize your workflow.  But at least when you get to this point you will have a frame of reference.

Knowing this, lets move onto how I setup Atom for my development workflow.

## My Text Editor Setup

As mentioned, `Atom` is _currently_ my preferred text editor for Clojure development.  The reason? it's portable, easy to setup and customize.

<aside class="blog-content__note">My Atom setup can be found below, but if you find video tutorials more helpful checkout my youtube video series <a class="blog-content__link" target="_blank" rel="noopener noreferrer" href="https://www.youtube.com/playlist?list=PLaGDS2KB3-AqeOryQptgApJ6M7mfoFXIp">Setup Atom for Clojure Development</a> where I go through everything from installing Atom to installing, configuring and demoing each tool I use.</aside>

### Plugins and Configuration

I have always found that to be productive with Clojure you don't need many tools. This is great because it means I can keep a relatively spartan setup for my Text Editor.  Now, let's take a look at the plugins I use and how I configure them.

<aside class="blog-content__note">For each of the plugins listed below you will have to install them.  If you have never installed packages with Atom it's straightforward, but if you need additional help <a class="blog-content__link" target="_blank" rel="noopener noreferrer" href="https://flight-manual.atom.io/using-atom/sections/atom-packages/">Checkout this guide</a>.
</aside>

- [Ink](https://atom.io/packages/ink)

  - Ink only required if your using a version of Chlorine under ` 0.7.2`.  Having said this, it doesn't hurt to have Ink installed because a lot of other Atom plugins require it anyways

  - **Description:** Chlorine depends on this.
  - **Configuration:** None required.

- [Chlorine](https://atom.io/packages/chlorine)

  - **Description:** Integrate your Clojure REPL into your editor.
  - **Configuration:** Add the Chlorine hotkeys.  [Here is an example](https://github.com/athomasoriginal/dotfiles/blob/master/atom/keymap.cson#L34) of where to put them.

- [Parinfer](https://atom.io/packages/parinfer)

  - **Description:** Automatically balance your parens.  Translation?  Thinks less about your parens.
  - **Configuration:** The default settings are great, but I recommend enabling `smart mode`


## Conclusion

Remember that no matter what language you choose, there are going to be a ton of micro decisions to make.  The important thing in the beginning is to focus on the language and the learning process and not stress over the tooling.  Be good to yourself in your learning journey and try not to obsess over all the details or aligning to the _ideal programmer_ stereotype.


<aside>
  <h3>Footnotes</h3>
  <ol>
    <li id="popular-editors">
      This list is based on the <a class="blog-content__link" href="https://clojure.org/news/2020/02/20/state-of-clojure-2020" target="_blank" rel="noopener noreferrer">2020 State of Clojure Survey</a>.
      <a href="#popular-editors-ref" aria-label="Back to content">Back</a>
    </li>
  </ol>
</aside>
