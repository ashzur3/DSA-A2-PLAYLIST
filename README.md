Data Structure & Algorithms
Assignment 2: MySongPlayer

Your company is developing a new program to stream songs. For this reason
you were asked to implement some of the functionalities that allow to manage
the playlists of this new software.
The main entity of the software you are developing are songs. A song consists
of a struct which has three fields, id, title, and duration. Where id is an integer
that uniquely identifies a song, title is the title of the song, and duration is a
float that specifies the duration of the song in seconds.
This is a general explanation of how a playlist should behave: You can think
of a playlist as a dynamic sequence of songs. Songs can be added to the end of
the sequence using the function addSong. A playlist will be used by the program
to keep track of which song should be played next. To do so the user program
will call the playSong function. Unless the playlist was modified (see below)
songs are usually played in the same order in which they were added.The user
program is also allowed to skip songs using the skipSong function. Once all the
song are played or skipped the playlist will restart playing from the fist song.
The user program can also start play the playlist from any given position in the
sequence using the function playFrom. Moreover, the playlist has two modes
of play songs: skip mode in which songs that were played at least once before
are skipped, and normal mode in which all the songs in the playlist are palyed
unless they re explicitly skipped. The user program can change the play mode
using the function skipAllPlayedSongs. Finally, the user program can modify
the playlist using the function swapSongs which allows to change the order of
two songs in the playlist.

Since your program will be part of a larger project the software engineer
of your company developed an interface for the library that you will have to
develop. You can find the interface of your library in the file “playlist.h” which
also contains the song type. This is a screenshoot of the playlist interface:
You should implement the playlist interface. In your implementation
you may assume that playlists are very static, i.e., most of the songs will be
added right after the playlist is created and the addSong function will rarely be
called after this initial phase.

Write a short (max 1 page) report where you explain an justify the
following implementation choices: [5 pts]
• the data structures you used to implement a playlist. [2 pt.]
• your implementation of playSong and playFrom. [3 pts.]

Your program should consist of one C file called “yoursurname.c” which
implements the interface “playlist.h”. Your program will be compiled using
“gcc -Wall -pedantic -std=c11 tester.c yoursurname.c -o test” where “tester.c”
is a program that will randomly generate and use your playlist. Your program
will then be tested 5 times with different testing parameters each passed test
is worth 1 point for a maximum of 5 points. You can find the “tester.c”
program on Canvas together with few examples of the expected output. You
can upload your program on Canvas and give me your report in class.
Deadline on the 22nd of November at midnight.

