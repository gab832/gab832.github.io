---
title: 'My First Post'
date: 2024-05-16T20:08:14+02:00
draft: true
---


if __name__ == “__main__”:

It is a shame but I did not know what this statement was for. Actually it is something basic that I had known, but I do not. After doing many technical interviews I found out a few things that I must know, including this one. You could learn from anyone and from any situation, so as an advice, try to learn each thing or question that you did not answer correctly in the interview.

Let’s go to what matters, the __name__ variable. This variable is set to ‘__main__’ when it is read from standard input, some script or from an interactive prompt. This value is the name of the scope in which top-level code executes. So checking that value we could know whether it has been executed or imported. This means that we could add some logic in purpose when the module is executed and when it is imported.

Examples:

module1.py

def main():
	run main
	print(“Main run”)

def import_logic():
	run logic
	print(“Import logic run”)

if __name__ == "__main__":
    # execute only if run as a script
    main()
else:
    # imported
    import_logic()


module2.py
import module1

python module2.py
Because the module1 is imported in module2, we go through the import logic.

python module1.py
Because module1 is executed directly, the __name__ variable will be __main__, so it will go through the if.

https://docs.python.org/3/library/__main__.html
