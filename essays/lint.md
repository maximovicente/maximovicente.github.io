---
layout: essay
type: essay
title: "Bringing Order to Order"
# All dates must be YYYY-MM-DD format!
date: 2026-09-24
published: true
labels:
  - ESLint
  - Coding Standards
  - Open Source
  - ICS 314
---

## Form Follows Function() {};

After understanding the overarching structure and ruleset of programming, learning new languages becomes a matter of memorizing language-specific syntax, operators, type constraints, and standard methods or classes provided by built-in libraries. This means developers, at some point, *should* be able to read and comprehend code in languages they have not written yet, provided the language follows much of the same syntactic ordering and keywords as the language(s) they are used to. The asterisk resides in whether or not that code was *intended* to be read, either by choice of the developer to obfuscate, or as a side effect of their unintelligible coding style. Clearly, just having code that *works* is not enough for open-source publishing, just as *law* is not enough for a healthy society—unwritten rules pertaining to morality and well-mannered conversation are essential. Luckily, in a system as deterministic as code, this extra layer need not go unwritten. We start with the idea that code can be divided into two groups: code meant to be read, and code not meant to be read. With such a dichotomous distinction, there must be a fine, objectively measurable line that separates the two. And it must be distinct, even orthogonal, from the compile-time rules that dictate whether or not the code will *run*. 

## Compilable vs. Committable

Enter coding standards. In the world of open-source software, I believe adherence to styling standards and linting should be the expectation, not a suggestion. Any code you publish that is meant to be seen, fixed, copied, adapted, or imported depends on that code being readable by a wide range of programmers from different schools, countries, or backgrounds. This requires an established rulebook that is agreeable to the greater part of a language's user base and, perhaps more importantly, can be implemented programatically in some readily apparent fashion, like error highlighting within an IDE. The latter point is not just a matter of convenience, but a stepping stone toward realistic, widespread adoption. Few programmers are willing to flip between a styling standard's official documentation and their code, rigorously checking every rule.

This, in my opinion, is why ESLint is **essential** for JavaScript programmers, and individual styling suggestions so elusive. ESLint is built on automatic, configurable fixes to coding practices, making linting extensions and utilities its intended application. After all, if the compilable syntax of a programming language is itself deterministically programmatic, why shouldn't coding standards be programmable, too? Otherwise, all you have is a set of rules where each programmer applies a potentially disjoint subset of those rules, and open-source software descends into the chaos of subjectively interpreted inconsistency. It's hard to call *that* a **standard**.

The best part is that we *all* reap the rewards of easy implementation. Even end users, who might never see the source code of a program they use, are ultimately better off for that software consistently adhering to coding standards, open-source or not. Regardless of *who* sees the code and fixes bugs, patches vulnerabilities, or adds features, having a well-defined set of standards for its organization, and making them automatically detectable, means updates can be made and published faster and with a lower risk of overlooking accidentally introduced bugs.

What we end up with is effectively a principle parallel to "Don't Repeat Yourself" (DRY), tailored to open-source software. I'm not sure I have a handy acronym for this one, but it is simple enough to remember without one: **Lint your code before committing it!** 

## Beyond the Compiler

Now, as we enter the age of AI-assisted programming, it may be time to emphasize our demand for reliably linted code from LLMs. Current models continue to be unreliable in this aspect, while some may even circumvent stylistic rules intentionally. If generative models are to be the programmers of the future, we should strive to train them on coding standards and readability, lest our software transforms into a mysterious black box, much like the models we use to generate it.