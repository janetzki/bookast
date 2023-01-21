![bookast](https://user-images.githubusercontent.com/57623556/212183761-79985c04-6a2d-4b3d-8a75-2f6fdcb19d3a.png)

# bookast: ChatGPT Podcast Generator For Books

## About
This project uses [ChatGPT](https://openai.com/blog/chatgpt/) to generate podcasts about books. We are using the [chatgpt-wrapper](https://github.com/mmabrouk/chatgpt-wrapper) library to interact with the ChatGPT API.


## Installation
1. Clone this repository.
2. Install the required dependencies:
```pip install -r requirements.txt```
3. Before starting the program, you will need to install a browser in playwright (if you haven't already). The program will use firefox by default.
```playwright install firefox```
4. With that done, you should start up the program in install mode, which will open up a browser window.
```chatgpt install```

## Usage
1. Enter your Replicate API token into bookcast/config.toml.

2. Run the generate_podcast.py script:
```python bookast/generate_podcast.py --book-name <book-name> --topics-number <topics-number>```

## Example
To generate a podcast about the book "The Alchemist" by Paulo Coelho, run the following command:
```python bookast/podcast/generate_podcast.py --book-name "The Alchemist" --topics-number 2```

## Output
The script will generate an audio file podcast.mp3 in outputs folder under data folder. This file will contain a podcast about the specified book, generated by ChatGPT.

## License
This project is licensed under the MIT License. See LICENSE for more details.
