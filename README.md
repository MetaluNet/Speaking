# Pd Speaking
** A library to make your pure-data patches speak, using a database of wav files. **

## Description
Speaking allow building a speech program by connecting elementary **say** blocks. Each **say** plays one of the user's soundfiles (a "phrase"), then triggers the next block. The soundfiles have to be organized in a precise tree structure, in the same way as the proposed example:

```
myspeech-wavs/
├── jack
│   ├── goodbye
│   │   ├── 1.wav
│   │   ├── 1.wav
│   │   └── ...
│   ├── hello
│   │   ├── 0.wav
│   │   └── ...
│   └── thanks
│       ├── 0.wav
│       └── ...
├── joe
│   ├── goodbye
│   │   ├── 0.wav
│   │   └── ...
│   ├── hello
│   │   ├── 0.wav
│   │   └── ...
│   └── thanks
│       ├── 0.wav
│       └── ...
├── phrases.txt (must contain the list of the phrases to use, one by semicolon terminated line)
└── voices.txt  (must contain the list of the voices to use, one by semicolon terminated line)
```

Open speaking-help.pd for example of use.

## Dependencies

PureData (version 0.48 minimum) + externals :

-	iemlib 
-	hcs 
-	ggee 


## Author

Antoine Rousseau <antoine@metalu.net> 2018  
license : GNU GPL (see [LICENSE.txt](LICENSE.txt) )
