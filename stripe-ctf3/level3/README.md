# Stripe CTF3: level3

## Description

[`git grep`](https://www.kernel.org/pub/software/scm/git/docs/git-grep.html) is nice and convenient for finding code in a single repository on your current disk. [Google Code Search](http://en.wikipedia.org/wiki/Google_Code_Search), and now [GitHub Code Search](https://github.com/blog/1381-a-whole-new-code-search), have shown how great it is to be able to search across all of your code at once.

But what if you want to search across all of your on-disk code? Ideally, there’d be a tool which indexes all of it for you, allowing you to perform instant search. For very low latency (which would allow cool things like typeahead search), you might distribute that work across multiple machines.

Any guesses where this is going? :)

For this level, you’ll be building a distributed instant code search. We’ve provided [a skeleton of a code search system written in Scala](https://github.com/ctfs/write-ups/tree/master/stripe-ctf3/level3/problem) for you; it’s too slow for anyone to be happy calling it instant code search though. Your job is to get queries to complete with much lower latency.

## Write-up

One solution is to implement a path-sharded in-memory scan.

(TODO)

## Other write-ups or solutions

* <http://muehe.org/posts/stripe-ctf-3-writeup/>
* <http://tullo.ch/articles/stripe-ctf-golfing/>
* <https://github.com/henrik-muehe/level3>
* <https://github.com/metcalf/ctf3/tree/master/level3>
