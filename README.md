# LordGPT
Autonomous AI Assistant fully capable of performing tasks on its own.

The bundle still requires that you have an OpenAI and Google Search key.

OpenAI API: 
1. Sign up for OpenAI; the first $15 is free: https://platform.openai.com/account/api-keys
2. Once logged in, click your profile in the upper right.
3. Choose "API Keys."
4. Generate an API key and save it somewhere; you won't be able to see it again.

Google Search API:
1. Sign up for a Gmail account if you don’t already have one. 2. Visit https://cloud.google.com/.
3. Go to "API & Services" and choose "Credentials."
4. Choose "Create Credentials" at the top and select "API key."
5. Save the API in Notepad, along with the OpenAI key.
6. Now visit the left menu again, select "API & Services," and choose "Enabled API & Services."
7. At the top of the page, select "+Enable API and Services."
8. In the search type "Custom Search."
9. Enable the API and choose "Manage."
10. Now visit Programmable Search - All search engines (google.com).
11. Click "Add" and give your search engine a name and select "Entire web," then click "Create."
12. Now copy the code after "cse.js." Example: "ccse.js?cx=e14a5ff417c4b26"

Choose "GPT-3.5-Turbo" unless you have GPT-4. Note: You’ll get errors if you try GPT-4 without access.

WELCOME LordGPT is an automated AI Assistant that can accomplish a wide range of tasks.
- Browse Internet and Research.
- Read and Write local files.
- Generate Python Scripts, and even write its own commands to further is capabilities.
- Search Google
- Generate formatted PDF Reports
- Use more than one API at a time. Options to flip between Azure and OpenAI for each call, reducing timeouts, and helping Azure and OpenAI out by spreading out requests.

LordGPT is different from other AI agents. I designed it not with code, but with prompt engineering. The code is simple as you can tell. The prompts are formatted to perform the tasks, not code. Hundreds of hours were spent on these prompts, and the slightest change will throw him off, keep that in mind. Also, I choose not to use the OpenAI module, and build from scratch to increase speed, even if its a few ms. Other than that, I hope you enjoy it as much as I did creating it.

COMING SOON:
Releasing a binary shortly to run LordGPT directly on windows without any of the steps below. Check back.

KNOWN ISSUES:
1. My python code is not optimized, no need to tell me. Join and help or post an issue.
2. Hallucinates and pretends to do things when the goal is too vague. I'm mostly fixed this but it happens randomly. Decrease the temp and top_p helps.
3. API Timeouts, nothing I can do. Apply for Azure GPT-4 and use the new ALTERNATE feature.Works great..
4. The prompts were built with my thinking mind, with that said you might prompt it to do things I didnt think of.


REQUIREMENTS:
- Google Search API for searching.
- Deep pockets for tokens.

MANUAL WINDOWS INSTALL
1. Enable WSL dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
2. Install WSL by running the following command: wsl --install
3. Follow the on-screen instructions to install your desired Linux distribution from the Microsoft Store.
4. Launch the Linux terminal by searching for your distribution or type WSL in the cmd prompt.

RUN THESE BASH COMMANDS, COPY AND PASTE
1. ls /home/USERNAME you choose during installation to see the files in your home directory.
2. Type sudo apt update && sudo apt upgrade && sudo apt install pip && sudo apt install wkhtmltopdf
3. type git clone GITURL
4. cd LordGPT
5. pip install -r requirements.txt - Sorry for the long requirements, its my dev machine.
7. python3 LordGPT.py


