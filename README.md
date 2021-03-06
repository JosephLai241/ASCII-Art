    ____________________________
    ________    |__    |_  ____/
    _______  /| |_  /| |  / __  
    ______  ___ |  ___ / /_/ /  
         /_/  |_/_/  |_\____/   

![GitHub top language](https://img.shields.io/github/languages/top/JosephLai241/AAG?&logo=Python)
[![Travis (.org)](https://img.shields.io/travis/JosephLai241/AAG?logo=Travis)][Travis Build]
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/JosephLai241/AAG/Pytest?logo=Github)][Github Actions - Pytest]
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/JosephLai241/AAG)][Releases]

# Table of Contents

* [Introduction](#introduction)
* [Walkthrough](#walkthrough)
    + [List All Available Fonts](#list-all-available-fonts)
    + [Generate Examples for All Fonts](#generate-examples-for-all-fonts)
    + [Generate Custom ASCII Art](#generate-custom-ascii-art)
    + [Generate ASCII Art From a Random Font](#generate-ascii-art-from-a-random-font)
* [Additional Help](#additional-help)

# Introduction

This is an ASCII art generator written in Python ([`pyfiglet`][PyFiglet]).

I wanted to make some ASCII art for my Raspberry Pi's MOTD and wondered if I could program something in Python that could generate it for me. I did some Googling and found `pyfiglet`, which is a full port of [FIGlet][FIGlet] into Python and would allow me to make such a program. 

I figured I could recreate it into a tool like [URS][URS] and put it on my profile, so here is the final product. ***Enjoy!***

# Walkthrough

There are four flags you can use with this program: `-l`, `-e`, `-m`, and `-r`.

## List All Available Fonts

`$ ./AAG.py -l`

Use this flag to see a list of all available fonts and their corresponding number. You will need the number to create your ASCII art.

## Generate Examples for All Fonts

`$ ./AAG.py -e`

This flag will provide examples for each font. 

## Generate Custom ASCII Art

`$ ./AAG.py -m FONT_NUM TEXT`

This flag is used to generate your ASCII art.

It takes 2 arguments - the font number and the string you want to generate art for.

## Generate ASCII Art From a Random Font

`$ ./AAG.py -r TEXT`

If you're feeling adventurous, let AAG choose the font for you.

# Additional Help

`$ ./AAG.py -h`

Use the help flag to see example usage and additional help.

<!-- BADGES -->
[Travis Build]: https://travis-ci.org/github/JosephLai241/AAG
[Github Actions - Pytest]: https://github.com/JosephLai241/AAG/actions?query=workflow%3APytest
[Releases]: https://github.com/JosephLai241/AAG/releases

<!-- LINKS -->
[PyFiglet]: https://pypi.org/project/pyfiglet/
[FIGlet]: http://www.figlet.org/
[URS]: https://github.com/JosephLai241/URS