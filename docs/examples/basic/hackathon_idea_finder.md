# Coffee Finder

This agent network looks for Hack Ideas options for its user,
depending on Areas chosen.

It's good for testing:

* how multiple agents can provide the same service
* how to leverage AAOSA instructions to
  * Disambiguate
  * Choose the best option depending on the context

## File


[hackathon_idea_finder.hocon](../../../registries/basic/hackathon_idea_finder.hocon)

## Description

Idea Finder is an agent network that can suggest options for Idea depending on Areas chosen..

## Example conversation

```text
Human:
Where can I find hack ideas?

AI:
you can find ideas based on Areas Choses
If you need specif idea at a specific time or more details, please let me know.
```

Following-up: 

```text
Human:
It's great.

AI:
may i help you more
```
