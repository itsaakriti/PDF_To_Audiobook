# Designing a PDF Audiobook using Python
In this code, a simple implementation of PDF Audiobook is shown. PDF text is read to the user as audio using this code.

#### Introduction
Sometimes reading books and huge essays from screen becomes a very tedious task,however if the same text is being read in an audio format becomes interesting and doesnt require as much concentration as reading requires. 
In this project, I have tried to implement a simple PDF to audio converter. This code scans page(s)[Proided the range of pages] of PDF and reads it using audio, to the user. 
While this project is good for simple text reading, it does not perform good if a scientific paper with complex/mathematical equations is given to it because equations are not 
supported in the pytesseract OCR library which I have used to convert Image to text.

#### Project Flow
Here is the project flow diagram:

![project flow](https://github.com/shayanalibhatti/PDF_text_to_audio_converter/blob/master/audiobook%20image.png?raw=true)

1) First, we take the PDF file ask the user for the range of pages they want to read and then convert each page into image using PyMuPDF software.
2) Then, we take the image(s) and scan the text in the image using Pytesseract OCR software.
3) Then, we use Google Text to Speech (gTTS) library to convert text to audio file.
3) Lastly, we get the Pygame mixer to play the audio file loud.

#### Prerequisite software
The software libraries/packages required to run this code can be installed using:
1) pip install Pillow -------- image reader library
2) pip install PyMuPDF ------- library to convert PDF page to image
3) pip install pytesseract --- Image to text converting Optical Character Recognition library
4) pip install pygame -------- pygame to play audio
5) pip install gTTS   -------- Google Text To Speech
6) pip install pysimplegui --- This library makes GUI development far simpler than tkinter.

#### Conclusion
It is seen that the code performs really well in reading straightforward PDF text files, however, if equations or any other text apart from english sentences are involved in the text, 
then the reader cannot properly read the equations.
Hence, the code is good for simple text but not for scientific papers as it will fumble and make no sense to the listener reading the equations. However, Simple text will be read just fine. 

#### Future Work
This code can be extended to make a book reading software or combined with machine learning to make really interesting story reader with interactive sounds based on situation 
depicted in the text.
