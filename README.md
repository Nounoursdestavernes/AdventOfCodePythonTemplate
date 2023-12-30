# DEPRICATED

I'm now working on a package named "PyAOC" doing the same things and more.

If you want to see the project go on :
[PyAOC](https://github.com/Nounoursdestavernes/PyAOC)


# AdventOfCodePythonTemplate

This repository is a template for solving the [Advent of Code](https://adventofcode.com/) challenges in Python. The template is designed to be as simple as possible, so you can focus on solving the challenges. It also includes a script to create the folders for each day and a script to create the README.md file with the links to the challenges and the solutions. It also benchmarks the solutions and adds the execution times to the README.md.


## Getting Started
To use this template, you need to clone this repository and install the requirements. It is recommended to use a virtual environment to install the requirements.

```bash
pip3 install -r requirements.txt
```

## Usage
To use this template, you need to create a new folder for each day. You can do this manually or by using the create_day.py script. 

### Create a day folder
```bash
python3 create_day.py <day>
```
This will create a new folder for the given day and prepare it for solving the challenges. It will create 

It will create a folder for the given day and prepare it for solving the challenges. The folder will have the following structure :
```
day/
  └ inputs/
    └ input.txt
  └ Part1/
    └ part1.py
  └ Part2/
    └ part2.py
  └ launcher.py
```
You have to put the input of the day in the input.txt file. You can find the input of the day on the [Advent of Code](https://adventofcode.com/) website.

You will have to write the code for each part of the challenge in the part1.py and part2.py files. You can use the launcher.py script to run the code for a specific part of the challenge.

### Running the code
To run the code for a specific day, simply run the launcher.py script with the path of the input of the day as an argument. You have to be in the day folder to run the script.
```bash
python3 launcher.py <filename>
```
This script have other options, you can see them by running:
```bash
python3 launcher.py -h
```

## Configuration
To use more advanced features, you need to configure the template. You can do this by editing the [config.ini](./config/config.ini) file. You can see an example of the configuration file in [example.ini](./config/example.ini). The configuration file is divided in sections. Each section is used to configure a day. The name of the section is the day of the challenge. Each section have the following arguments:
- **name**: The name of the challenge (mandatory)
- **res_part1**: The expected result of the part 1 of the challenge (optional)
- **res_part2**: The expected result of the part 2 of the challenge (optional)

This configuration unlocks the following features:
- **assert**: If the expected result is given, the launcher.py script will assert that the result of the code is equal to the expected result.
- **benchmark**: The create_readme.py script will benchmark the code and add the execution time to the README.md file.

## Create the README.md
To create the README.md file, simply run the create_readme.py script.
You must have configured the template to use this script.
```bash
python3 create_readme.py
```
This will create the README.md file with the links to the challenges and the solutions. It will also benchmark the solutions and add the execution times to the README.md. It will also benchmark the solutions and add the execution times to the README.md.
You can modify the [README.md](templates/README.jinja2) template.

## License
This project is licensed under the Mozilla Public License 2.0 - see the [LICENSE](LICENSE) file for details.
