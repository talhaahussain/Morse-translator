# Morse-translator
A Morse code translation tool, written in Haskell.

### Usage (with GHCi)

#### GHCi and Loading Modules

First, run `ghci` to enter The Glasgow Haskell Compiler interactive interface. Load the source files with 

```
Prelude> :l morse_to_text.hs
```
and
```
Prelude> :l text_to_morse.hs
```

#### Translating Morse to Text

Translating Morse code to plaintext can be done either with a single Morse string or an array of Morse strings. To translate a single Morse string, use

```
Prelude> morseToChar ".-" 
```

To translate a sequence of Morse strings, use

```
Prelude> morseToString ["....", ".", ".-..", ".-..", "---", "     ", ".--", "---", ".-.", ".-..", "-..", "-.-.--"]
```

#### Translating Text to Morse

Translating plaintext to Morse code can be done either character-wise or string-wise. To translate a single character, use

```
Prelude> charToMorse 'A'
```

To translate a string, use

```
Prelude> stringToMorse "Hello World!"
```
