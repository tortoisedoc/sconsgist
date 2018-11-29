import os

# Set the directory you want to start from
rootDir = '.'
staged_dir = "stage"

for dirName, subdirList, fileList in os.walk("./src"):
  for filename in fileList:
    if filename == "SConscript":
      sconScript = os.path.join(dirName, filename)
      print ("Found %s " % sconScript)
      SConscript(sconScript, variant_dir=os.path.join(staged_dir, dirName), duplicate = 0)
