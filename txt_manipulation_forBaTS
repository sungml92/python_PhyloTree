#BaTS analysis is useful to analyze tip-to-phylogeny association
#The jar software requires specific file format that needs "cleaning" of BEAST posterior tree

'''
This require you to import re to begin with
Also, you should define the name of discrete Trait in pName below
For example, if you set your discrete Trait as Species
-> pName = "Species"
'''

#Set your name of discrete trait
pName = "Location"

import re
handle = open(path-to-posterior-tree-file,"r")
file = handle.read()

toR = [
    ("\[\&default.+?\]",""),
    ("\[\&%s.+?\]" % pName,""),
    ("\[\&joint.+?\]","")
]

for target,outcome in toR:
    cleanfile = re.sub(target,outcome, file)

with open(Path&Name-to-save,"w") as f:
    f.write(cleanfile)
