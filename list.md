# Steganography - A list of useful tools and resources

## Steganography

CTF steganography usually entails uncovering the steganographically hidden hints or flags (most commonly a media file). A basic understanding of media filetypes (e.g., jpg, bmp, png for photos and wav, mp3 for sound) is necessary for steganography, as it is crucial to understand how files can be concealed and masked. Also, because a variety of tools operate in a Linux shell, it's vital to have a basic understanding of Linux.

Here's a list of the tools I use the most, as well as some other resources.

## Tools

## Steghide

Steghide is a steganography tool that hides data in a variety of image and audio files. It only supports `JPEG, BMP, WAV, and AU files`. However, it can also be used to extract embedded or encrypted data from other files.
It can be installed using `apt`, however the [source](https://github.com/StefanoDeVuono/steghide) is available on github.

Useful commands:
</br>
`steghide info file`: displays info about a file whether it has embedded data or not.
</br>
`steghide extract -sf file`: extracts embedded data from a file.

## Foremost

I found it useful while dealing with png images. Foremost is a programme that recovers files based on their headers, footers, and underlying data structures.
It can be installed using `apt`, however the [source](https://github.com/korczis/foremost) is available on github.

Useful commands:
</br>
`foremost -i file`: extracts data from the given file.

## Stegsolve

In other cases, a message or text is hidden within the image, and in order to see it, you must use colour filters or play with the colour levels. GIMP, Photoshop, or any other image altering software can be used, however stegsolve makes things easier. It's a little Java program that lets you apply a variety of colour filters to photos. Personally, I find it quite beneficial. </br>
Stegsolve is available on [github](https://github.com/eugenekolo/sec-tools/tree/master/stego/stegsolve/stegsolve).

## Strings

Strings is a linux command-line programme that shows printable strings in a file. When it comes to steganography challenges, this basic tool can be really useful. Embedded data is usually password protected or encrypted, and the password is occasionally stored in the file itself and can be easily viewed using strings. You don't need to install anything because it's a standard linux program.

Useful commands:
</br>
`strings file`: displays printable strings in the given file.
