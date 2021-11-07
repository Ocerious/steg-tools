# Steganography - A list of useful tools and resources

## Steganography

CTF steganography usually entails uncovering the steganographically hidden hints or flags (most commonly a media file). A basic understanding of media filetypes (e.g., jpg, bmp, png for photos and wav, mp3 for sound) is necessary for steganography, as it is crucial to understand how files can be concealed and masked. Also, because a variety of tools operate in the Linux shell, it's vital to have a basic understanding of Linux.

Here's a list of the tools I use the most, as well as some other resources.

## Tools

## Steghide

Steghide is a steganography tool that hides data in a variety of image and audio files. It only supports `JPEG, BMP, WAV, and AU files`. However, it can also be used to extract embedded or encrypted data from other files.
It can be installed using `apt`, however the [source](https://github.com/StefanoDeVuono/steghide) is available on Github.

Useful commands:
</br>
`steghide info file`: displays info about a file whether it has embedded data or not.
</br>
`steghide extract -sf file`: extracts embedded data from a file.

## Foremost

I found it useful while dealing with png images. Foremost is a programme that recovers files based on their headers, footers, and underlying data structures.
It can be installed using `apt`, however the [source](https://github.com/korczis/foremost) is available on Github.

Useful commands:
</br>
`foremost -i file`: extracts data from the given file.
