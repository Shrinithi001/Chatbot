# Chatbot
from tkinter import *
root=Tk()

def send():
    send = "You:" + e.get()
    text.insert(END, "\n" + send)
    if (e.get() == 'hi'):
        text.insert(END, "\n" + "Bot: hello")
    elif (e.get() == 'hello'):
        text.insert(END, "\n" + "Bot: hi")

    elif (e.get() == 'how are you?'):
        text.insert(END, "\n" + "Bot: i'm fine and you?")

    elif (e.get() == "i'm fine too"):
        text.insert(END, "\n" + "Bot: nice to hear that")

    elif (e.get() == 'Is the college affiliated to a university or autonomous?'):
        text.insert(END, "\n" + "Bot: College is affiliated to University")

    elif (e.get() == 'Average CGPA of students year wise'):
        text.insert(END, "\n" + "Bot: Average CGPA is 8.5")

    elif (e.get() =='Which companies have visited the college for placement?'):
        text.insert(END, "\n" + "Bot: Top recruiting Companies with high packages have visited")

    elif (e.get() =='Last year’s highest placement package?'):
        text.insert(END, "\n" + "Bot: 24LPA")

    elif (e.get() =='What is the minimum package given?'):
        text.insert(END, "\n" + "Bot: 7 LPA")

    elif (e.get() == 'Is bus transport is compulsory?'):
        text.insert(END, "\n" + "Bot: Yes,Bus is Compulsory")

    elif (e.get() =='What are the extracurricular activities provided in college?'):
        text.insert(END, "\n" + "Bot:Student Council,Sports,Activities in Clubs & Socities")

    elif (e.get() == 'Are phones allowed inside the college campus?'):
        text.insert(END, "\n" + "Bot:Yes,but using Phone during class hours is prohibited")

    elif (e.get() == 'What type of accreditation the college has?'):
        text.insert(END,"\n" + "Bot: There are three types of accrediting bodies: regional, national, and programmatic ")

    elif (e.get() == 'How many and what are all the clubs in the college?'):
        text.insert(END, "\n" + "Bot: 7 Clubs.Art,Language,Coding,Cultural,Sports,NCC,NSS,Media")

    elif(e.get() =='Is there any scholarships?'):
        text.insert(END, "\n" + "Bot:Yes, There are many scholarships available")

    elif(e.get() =='Will every student’s progress be mentored?'):
        text.insert(END, "\n" + "Bot: Yes,Every students have an individual mentors")

    elif(e.get() =='Is there a full facilitated library?'):
        text.insert(END, "\n" + "BOt: Yes, we have a full facilitated and sophisticated Library")

    elif(e.get() =='How are the facilities in Hostel?'):
        text.insert(END,"\n" + "Bot:Hostel have such a good facilities with good drinking water and other leisure/sport timwe with reading")

    elif(e.get() =='What is the college timings'):
        text.insert(END,"\n" + "Bot: 9:00 am to 4:00 pm")

    elif(e.get()=='What are the new courses introduced?'):
        text.insert(END,"\n" + "Bot:Courses on AI,Cyber Security,IOT")

    elif (e.get() == 'What is Artificial Intelligence?'):
        text.insert(END, "\n" + "Bot: Artificial intelligence is the simulation of human intelligence by machines .")

    elif (e.get() == 'What jobs are available in AI?'):
        text.insert(END, "\n" + "Bot: Data scientist,Senior software engineer")

    elif (e.get() == 'What is Cyber Security'):
        text.insert(END,"\n" + "Bot:Cyber security is the practice of defending computers, servers,networks")

    elif (e.get() == 'What are the emerging courses'):
        text.insert(END,"\n" + "Bot:Entrepreneurship,Law,Engineering,Architecture")


    else:
        text.insert(END, "\n" + "Bot: Sorry I didnt get it.")


text = Text(root, bg='white')
text.grid(row=0, column=0, columnspan=2)
e = Entry(root, width=80)
send = Button(root, text='Send', bg='blue', width=20, command=send).grid(row=1, column=1)
e.grid(row=1, column=0)
root = Tk()
root.title('SAMPLE CHATBOT')
root.mainloop()
