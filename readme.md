# Funny Randomness

The usability of passwords is broken. This is a minimum viable prototype of a [mnemonic device](https://en.wikipedia.org/wiki/Mnemonic) to memorize strong passwords effortlessly.

It generates 'stories' of the format `[person1] [action] [person2]'s [object]`. The resulting stories are intended to provoke mental images that are funny or absurd, because humor is well known to be helpful for learning.

## Related Work

- [Bruce Schneier: Changes in Password Best Practices](https://www.schneier.com/blog/archives/2017/10/changes_in_pass.html)
- [Bruce Schneier: Choosing Secure Passwords](https://www.schneier.com/blog/archives/2014/03/choosing_secure_1.html)
- https://www.kaspersky.com/blog/remember-strong-passwords/6386/
- https://arxiv.org/pdf/1302.5122.pdf
- https://arxiv.org/pdf/1410.1490v1.pdf

## Word Lists
- Persons
	- Lists of persons or fictional characters that are known to most people (in the western world). 
- Actions
	- [English verbs](https://github.com/dariusk/corpora/blob/master/data/words/verbs.json)
- Objects
	- [Top 1500 nouns in english](http://www.talkenglish.com/vocabulary/top-1500-nouns.aspx) because the more common the nouns, the easier they are to memorize.

## Experiments

First results of the evaluation of this prototype:
- Users perceived the random stories to be funny.
- Users liked to generate stories.
- Users had individual emotional attachment to different stories.
- Users memorized the story 'well' when picking it by themselves.

## Limitations
This prototype is not secure. It is limited to only 10656188312 different stories which is way too easy to bruteforce. It is equivalent to a password consisting of 7 random lowercase chars in the range of a-z. Further prototypes and experiments with multiple or longer stories are necessary before using this approach in production.

## Conclusion
Mnemonics potentially solve the usability problem of passwords. For the average user it becomes easy to memorize randomly generated passwords. Though this prototype lacks entropy and therefore is not secure yet. This issue is probably solvable by a more sophisticated generation of stories.
