# nestesLoop



def main():
    fileName = input("What is the name of the file? ")
    total = 0
    count = 0
    infile = open(fileName, "r")
    line = infile.readline()
    while line != "":
        for xstr in line.split(","):
            total += float(xstr)
            count += 1
        line = infile.readline()
    print("Average of the numbers is", total / count)

main()
