# text-to-speech-python
A python project that requests text data and outputs audio mp3 data


Text to speech is the generation of speech synthesized from the text. The technology is used to communicate with users when reading a screen is not possible or impractical. This not only opens up apps and information to use in new ways but can also make the world more accessible to people who cannot read text on a screen. In this article, I will take you through building your TTS with Python.

I will simply start with importing all the necessary libraries that we need for this task to create a program that takes the text of an article online and converts it into speech:

#Import the libraries

Now, if you have face any error in importing the libraries, then you must have not installed any of these libraries. You can easily install any library in python, by writing a very simple command in your terminal – pip install package name. Now after installing and importing the libraries, we need to get an article from online sources so that we can create a program to convert text to speech from that article:

#Get the article

article.download()
2
article.parse()
Now you need to download the “punkt” package if you have already downloaded it before you can skip downloading it if you will still download it again, it will give you a reminder that it is already available in your system which will not harm anything. So now, I will download the punkt package and apply Natural Language processing on it:

Now, I will define a variable to store the article:

#Get the articles text
Now we have to choose the language of speech. Note “en” means English. You can also use “pt-br” for Portuguese and there are others:

language = 'en' #English
Now we need to pass the text and language to the engine to convert the text to speech and store it in a variable. Mark slow as False to tell the plug-in that the converted audio should be at high speed:

Running Text to Speech Program
Now, we have converted the article for text-to-speech, so now the next step is to save this speech to mp3 file:

myobj.save("read_article.mp3")
