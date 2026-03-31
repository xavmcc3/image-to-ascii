![image](img/banner.png)

# <image src="img/logo.png" width=37 style="vertical-align: middle;"> Image to ASCII

This python program takes in an input image and applies effects to it via a CLI.

## Setup

Clone the repo to get started, then navigate into the folder and run it with the `python` command.

## Usage

Run it with `python main.py -p <process> -u <url>`, where `<process>` is the type of effect to use and `<url>` is the url to the image.

 - `threshold_image` Convert the image to pure black or pure white binary.
 - `ascii_image` Convert the image to colored ascii characters.
 - `grey_hex_image` Convert the image to black and white with greyscale values.

Any output is stored in `data.txt` in the same directory.

## About
New effects can be added to the program using the `@process` decorator. The README *should* automatically update with each push to accomodate new processes.
```py
@process('description')
def example_process():
    pass
```

## Todo
In-progress .
 - [ ] render the ascii image to some sort of canvas (probably with PIL)
 - [ ] Cmd option for custom output filenames
 - [ ] file inputs ? i guess??
 - [ ] make it so I don't have to git pull after every push for the updated README
 - [ ] process-dependent parameters
 - [ ] fix longer width ascii images (cmd display only)
 - [ ] generate this section from the `json` file
 - [ ] fix dependencies
 - [ ] create `res` folder

