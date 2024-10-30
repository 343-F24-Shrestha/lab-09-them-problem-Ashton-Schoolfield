# Them Problem

## Motivation and Learning Objectives

You've been spinning asynchronous code for a while now, primarily as event listeners using callbacks.
In preparing to sling more complex asynchronous code, it would be helpful to have a few more cartridges in your utility belt.

By the end of this lab, you should be able to:
1. call functions that return promises
1. test functions that return promises
1. recognize that not every problem is yours, but that some problems are "theirs", "them problem"s if you will.

## Goal

Provided with the starting code from the template here or from your instructor, create something similar to this demo available for [mobile](https://youtube.com/shorts/emnjXqlUx_U) and [desktop](https://youtu.be/v5PAXPlFfgw). There are several "Them Problems" described by a pair of discordant emotional states in which "you" have a positive affect, but "they"have a negative affect, e.g. 

<ol>
<li><dl><dt>you</dt><dd>poppin'</dd><dt>they</dt><dd>stoppin'</dd></dl></li>
<li><dl><dt>you</dt><dd>packin'</dd><dt>they</dt><dd>lackin'</dd></dl></li>
</ol>

### Currently
In the provided starter code, the list of possible states "you" might be in comes from a call to a synchronous function (`getYous`) that immediately returns a short array of strings. Once one of these is selected, the starting code retrieves the corresponding state that "they" might be in when it's a "them problem" through a call to a synchronous function (`getThey`). This function also immediately returns, but only 1 string.

### Your task
1. replace the call to `getYous` with a call to `getOptions` which returns a promise that resolves to the array of strings.
1. replace the call to `getThey` with a call to `getThemProblem` which returns a promise that resolves to the string.

### Stretch Goals
1. invoke `toggleLoader` when appropriate to show the loading animation to give the visitor feedback that something is happening "in the background".