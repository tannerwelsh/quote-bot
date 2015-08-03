# Quote Bot

A program that generates **fake** quotes.

Quotes are generated from a specified corpus of work such that they "sound" as if they were generated by the author.

For example, quotes generated from a corpus of Bertrand Russell's work:

> A .... B .... C .... C .... Half the time may be performed however much.

> Differentiation; and that motion is really a means of distinction can be known by memory.

> Associations as the engram due to memory, and through the laws of dynamics. This is.

They don't always make too much sense.

> Wish to combat psychological theories of motion is continuous? It is generally supposed. When we.

## Usage

The `bot.py` script is the main executable, and can be used as such:

```shell-session
$ python3 bot.py <min sent length> <algorithm> <source>
```

For example, to generate a quote of at least 14 words using the Markov algorithm, sourced from all of the works in the `corpora/russell` folder:

```shell-session
$ python3 bot.py 14 markov corpora/russell/*
Must consist of simple parts, and there may be uniquely determined by their consequences just.
```

The other algorithm choice is `freq` and uses a probabilistic frequency distribution of words to generate quotes:

```shell-session
$ python3 bot.py 14 freq corpora/russell/*
Determining aspect to in our place than intrusion evident, character independence persistence power way is.
```
