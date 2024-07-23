# Python / Ollama RAG Demo

This is the code that we used in [the July 23 and August 23 The Scoop on Embedding: Teaching Large Language Models the “Flavor of the Day” at Culvers](https://events.nvisia.com/conference/be3edb0f-815e-48dd-9826-9b62f6fbc93a/schedule).  This is a command line interface (CLI) app but you can expand it to be a web service.  This should run on a Windows PC but these instructions assume that you are using MacOS.

## Steps to run this locally

1. [Install Ollama on your computer](https://ollama.com/download)
2. Pull down this project from [Github](https://github.com/steinbring)
3. Navigate to the project folder in [iterm2](https://iterm2.com/) (or Terminal)
4. Pull down llama3
	1. `ollama pull llama3`
5. Pull down nomic-embed-text
	1. `ollama pull nomic-embed-text`
4. Set up your Python virtual environment
	1. `pip3 install virtualenv` (if needed)
	2. `python3 -m venv ragdemo`
	3. `source ragdemo/bin/activate`
6. Install ollama, chromadb, and requests
	1. `pip3 install ollama`
	2. `pip3 install requests`
	3. `pip3 install chromadb`
7. Run the app (making an actual query)
	1. `python3 app.py "What is today's custard flavor at the Port Washington location?"`

## Are you having trouble running this?

Feel free to contact me on [Mastodon](https://jws.social/@joe) or [Signal](https://signal.me/#eu/wYx/v3zx0aPCt1RvLXBtCTcrKGWK0hJiIw2JpsQatK5UCSN9YMpDurXTeZ11atLj)
