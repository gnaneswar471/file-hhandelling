# file-hhandelling
fil=input("choose a file to access and read the data and display")
with open(fil,'w') as f:
    f.write("hello guyss\n")
with open(fil,'r+') as file:
    #file.seek(0)
    print("lattest data:",file.read())
    file.seek(0)
    user_input=input("enter text to overwrite")
    file.write(user_input)
    file.seek(0)
    print("\n file after wrting is r++\n",file.read())
OUTPUT:
choose a file to access and read the data and display anything.txt
lattest data: hello guyss

enter text to overwrite hi   

 file after wrting is r++
 hi    guyss

with open('line.txt','a+') as file:
    text=input("Enter a Line to append data:")
    file.write(text+'\n')
    file.seek(0)
    print("\n current content in the file. \n")
    print(file.read())
OUTPUT:
Enter a Line to append data: apparao

 current content in the file. 

hieeellell
heeloo
apparao
