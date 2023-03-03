## Extracting data from PDFs

These are supplementary files and instructions for a workshop I taught at NICAR 2023 in Nashville. If you attended, thanks for attending and keep in touch!

scottgpham[at]gmail.com

twitter: @scottpham

### Files you need

For now, simply download this whole repo. We'll use these PDFs for exercises during the workshop.

You will want to install the following free and open-source applications:

#### [Tabula](https://tabula.technology/)
A simple tool to extract data from "computer-generated" PDFs. Download the version for your operating system via the buttons on the top-right of the website:

![image](https://user-images.githubusercontent.com/7005290/222268945-20de397a-79fc-411e-9821-0243116be1ce.png)

#### [OCRmyPDF](https://ocrmypdf.readthedocs.io/en/latest/installation.html)
A simple command-line application to add an optical character recognition layer to a PDF.

Detailed installation instructions for any operating system are [available here](https://ocrmypdf.readthedocs.io/en/latest/installation.html).

For a mac, the easiest method is to install via Homebrew, a common package-manager for mac tools. 

`brew install ocrmypdf`

If you don't have Homebrew installed, you'll need to install Homebrew first before installing OCRmyPDF. Yes, I know, it's a bit convuluted. But trust me, it's a lot easier than installing "manually". Follow [this detailed guide](https://mac.install.guide/commandlinetools/3.html) or do the below:

1. Open your terminal (just type CMD + SPACE and search for "terminal" using spotlight).

2. Copy this line exactly as it's written and paste it into your terminal:

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Make sure there are no extra spaces or punctuation here or it won't work. 

3. The Homebrew installation script will ask you to enter your Mac user password. This is the password you used to sign into your Mac. You won't see the characters as you type. Press enter when you are done.

![image](https://user-images.githubusercontent.com/7005290/222271795-9d7771f5-6b94-4d8f-a8f7-9821ddf33125.png)

4. You may be prompted to install "X-Code Command Line Tools". This common somftware from Apple that many developer tools use. If it does prompt you, simply hit enter and XCode will be installed along with Homebrew. 

5. Wait for a several minutes while everything installs. You'll see a lot of wild looking text scrolling very fast on your terminal.  When it's finished, you'll be able to install OCRmyPDF with this terminal command: `brew install ocrmypdf`. Simply type that in and hit enter. 

6. If you get the message `zsh: command not found: brew` and you are using an Apple "Silicon" Mac, there is one more step you must take. You can follow instructions carefully [in the install guide](https://mac.install.guide/commandlinetools/3.html), or simply type the following into your terminal:
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

