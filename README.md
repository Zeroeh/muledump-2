###:Linux / macOS Users:
1. cd to wherever you'd like the project.
2. git clone https://github.com/Zeroeh/muledump-2
3. Wait for the download to finish and cd into the directory
4. Change the files as described in the windows section. You can rename files with `mv -n example_settings.json settings.json`
5. If you don't have go installed, run `sudo apt-get install golang && go build`. If you already have go installed, simply run `go build`. macOS users will need to install brew to run these commands.
6. Type `./muledump-2` or whatever binary go built.
7. Web server should be running, simply go to your browser `http://127.0.0.1:5353/muledump.html`

1. Download this repo, and extract the ZIP to your Desktop or another location. Name the folder `muledump-2-master`.
    For simplicity I'm going to assume you're going to put it in 
    C:\Users\Example\Desktop\muledump-2-master
2. Open your command prompt (Windows key+R, type in cmd.exe and hit enter)
4. Type in the following:
    `cd "C:\Users\Example\Desktop\muledump-2-master"`
5. If you do not want to build your own Go file, skip steps 5, 6 and 7.
6. Install Go from [here](https://golang.org/dl/).
7. Delete muledump-2-master.exe from your Muledump 2 folder, unless you want to keep it for some reason. (muledump-2-master.exe is the built main.go file)
8. In Command Prompt (you should be in C:\Users\<Your Name>\Desktop\<your Muledump 2 folder name>), type `go build`.
9. Open accounts_sample.js with a text editor (for instance Notepad++)
10. Enter your account info. Steam and Kong do not work as of now.
    It should look something like this: 

    accounts = {
    'me@example.com': 'example',
    }

11. Save the file as accounts.js (make sure it saves as a .js file, and not accounts.js.txt)
12. Open example_config.json with a text editor (for instance Notepad++)
13. Put in your email and password in there. For steam users, put in your steamworks user id and secret token.
    It should look something like this:
[
    {"user":"my@email.com", "password":"mypassword123"}
]

14. Save the file as config.json. Make sure the file extension is .json instead of .txt
15. Go back to your command prompt. Type in: 
muledump-2-master.exe "config.json"
16. Go to http://localhost:5353/muledump.html and click reload all.
