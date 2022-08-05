# sic-addons
Basically a place to show off addons for S.I.C.

S.I.C. is a project we are busy working on and this is kind of classified so you will need context to understand this.
Also the reason I'm making this public is so that I can download files without a token.

An addon is very basic, let me show you: (it's in python btw)
```
def getvar(text):
    if "<<<fact>>>" in text:
        if True:
            import random
            import os
        
            import requests
            g = requests.get("https://raw.githubusercontent.com/compactcoding-sa/sic-addons/main/facts/facts.txt").text
            return text.replace("<<<fact>>>",random.choice(g.split("\n")))
    else:
        return text
```
The getvar function is called to replace the text that calls the var with the actual var.
And now just rename it from `fact.py` to `fact.sicaddon`!
