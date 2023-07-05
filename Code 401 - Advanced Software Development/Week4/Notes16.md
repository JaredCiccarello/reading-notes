July 3, 2023

Sick Roger

  SERVERLESS FUNCTIONS

Docker container:
Everything is contained inside of that docker container
You can only change code that is inside that container

Virtual environment is similar to a docker container except docker is like a copy of the code.

Virtual environment is like a wrapper. 

Virtual machines are expensive, in terms of resources.


  Serverless World
People used to host servers and people would migrate to those.
Now they have found they can do without this.

Serverless function: "Lives on the internet and just does a thing"


restcountries.com
requests: HTTP for Humans
Most popular request in the world.
This is synchronous, must finish request before another is made.
asynchonrous is requests without previous being made.


  VERCEL
vercel.com/docs
documentation will help you to figure out how to do things.


If you're still getting an error code, look into THE FOLDER with a date.
add api/date to the end of the url

In your code, MUST have a return

self.mfile.write(formatted_time).encode()
This is wrong, it should be
self.mffile.write(formatted_time.encode())

This is saying to have the encode be inside

SETUP
mkdir speedrun
mkdir api
touch api/test.py
mv api/test.py api/ping.py
python3 -m venv .venv
touch .gitignore
gitignore: .idea .venv


ping.py
  class handler(BaseHTTPRequestHandler):
    def do_GET(self):
        self.send_response(200)
        self.send_header("Content-type", "text-plain")
        self.end_headers()

        message = "some text"

        self.wfile.write(message.encode())

pip install requests









TLDR: 
Virtual Environment
Docker Container
Serverless World
Vercel