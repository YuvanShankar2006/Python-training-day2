# Python-training-day2
class library:
    def __init__(self,bookname,serial_number,genre,author):
        self.bookname=bookname
        self.serial_number=serial_number
        self.author=author
        self.genre=genre

    def show(self):
        print(self.bookname)
        print(self.serial_number)
        print(self.author)
        print(self.genre)

    def addbook(self):
        self.bookname=input("Enter book name :")
        self.serial_number=int(input("Enter the serial number :"))
        self.author=input("Enter the author Name :")
        self.genre=input("Enter the Genre :")

    def searchbook(self):
        searching=input("Enter a book name to Search :")
        if(self.bookname==searching):
            print(f"Book is available in{self.genre}")

class sciencefiction(library):
    def __init__(self,bookname,serial_number,genre,author):
        super().__init__(bookname,serial_number,genre,author)
    
sfbook1=sciencefiction("November 9","1234","colleen Hoover","love")
sfbook2=sciencefiction("verity","1235","colleen Hoover","love")
sfbook3=sciencefiction("slammed","1236","colleen Hoover","love")
sfbook4=sciencefiction("Without Merit","1237","colleen Hoover","love")
sfbook5=sciencefiction("It ends with us","1238","colleen Hoover","love")

class comics(library):
    def __init__(self,bookname,serial_number,genre,author):
        super().__init__(bookname,serial_number,genre,author)
cobook1=comics("captain America","1239","stanlee","action")
cobook2=comics("Winter soldier","1240","stanlee","action")
cobook3=comics("iron man","1241","stanlee","action")
cobook4=comics("Thor","1242","stanlee","action")
cobook5=comics("Hulk","1243","stanlee","action")

class novels(library):
    def __init__(self,bookname,serial_number,genre,author):
        super().__init__(bookname,serial_number,genre,author)
nobook1=novels("harry potter","1244","JK rowling","Fiction")
nobook2=novels("fantastic beasts and where to find them","1245","JK rowling","Fiction")
nobook3=novels("godric hallows","1246","JK rowling","Fiction")
nobook4=novels("hermoine granger","1247","JK rowling","Fiction")
nobook5=novels("Ronald weasely","1248","JK rowling","Fiction")

class storybook(library):
     def __init__(self,bookname,serial_number,genre,author):
        super().__init__(bookname,serial_number,genre,author)
stbook1=storybook("fantastic four","1249","george","kids")
stbook2=storybook("fantastic four1","1250","julian","kids")
stbook3=storybook("fantastic four2","1251","annebelle","kids")
stbook4=storybook("fantastic four3","1252","reya","kids")
stbook5=storybook("fantastic four4","1253","sriram","kids")


print("Welcome to Yuvan's Library !")
print( "The book types are :")
print("(1) Science fiction books")
print("(2) Comics")
print("(3) Novels")
print("(4) Story Books")  
choice=input("Enter your choice from the List :").strip()
choice=choice.lower()
if(choice=="sciencefictionbooks"):
    sfbook1.show()
    sfbook2.show()
    sfbook3.show()
    sfbook4.show()
    sfbook5.show()
elif(choice=="comics"):
    cobook1.show()
    cobook2.show()
    cobook3.show()
    cobook4.show()
    cobook5.show()
elif(choice=="novels"):
    nobook1.show()
    nobook2.show()
    nobook3.show()
    nobook4.show()
    nobook5.show()
elif(choice=='storybooks'):
    stbook1.show()
    stbook2.show()
    stbook3.show()
    stbook4.show()
    stbook5.show()
else:
    print("invalid selection !")





    





       

      
    
