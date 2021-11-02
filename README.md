# solution-submission-
Trying to solve
project-A

int(input("enter your aadhar number"))

#creation of capcha 

from tkinter import *

from tkinter import messagebox

import random

text = 'abcdefghijklmnopqrstuvwxyz0123456789'

root = Tk()

root.title("Captcha verification App")

root.geometry("300x150")

captcha = StringVar()

input = StringVar()

def create_captcha():

c = random.choices(text, k = 5)

captcha.set(''.join(c))

def check():

if captcha.get() == input.get():

messagebox.showinfo('Captcha Verification', 'Captcha verified Succesfully..')

else:

messagebox.showerror('Captcha Verification', 'Incorrect Captcha')

input.set('')

create_captcha()

Label(root, textvariable=captcha, font="ariel 16 bold").pack(padx=5, pady=5)

Entry(root, textvariable=input, bg='white', font="ariel 12 bold").pack(padx=5, pady=5)

Button(root, text="Check", font="ariel 15 bold", bg='gold', command=check).pack(padx=5, pady=5)

create_captcha()

root.mainloop()

#asking for landlords aadhar number

Landlords_aadhar_number=(input("landlords aadhar number"))

#code for otp generation

#OTP generation 

# import library

import math, random 

 

# function to generate OTP

def generateOTP() : 

 

    # Declare a digits variable  

    # which stores all digits 

    digits = "0123456789" 

    OTP = "" 

 

   # length of password can be changed 

   # by changing value in range 

    for i in range(4) : 

        OTP += digits[math.floor(random.random() * 10)] 

 

    return OTP

#sending otp to send otp to register mobile number

import time 

from time import sleep 

from sinchsms import SinchSMS 

 

# function for sending SMS

def sendSMS(): 

 

    # enter all the details 

    # get app_key and app_secret by registering 

    # a app on sinchSMS 

    number = 'your_mobile_number' 

    app_key = 'your_app_key' 

    app_secret = 'your_app_secret' 

 

    # enter the message to be sent 

    message = 'Hello Message!!!' 

 

    client = SinchSMS(app_key, app_secret) 

    print("Sending '%s' to %s" % (message, number)) 

 

    response = client.send_message(number, message) 

    message_id = response['messageId'] 

    response = client.check_status(message_id) 

 

    # keep trying unless the status retured is Successful 

    while response['status'] != 'Successful': 

        print(response['status']) 

        time.sleep(1) 

        response = client.check_status(message_id) 

 

    print(response['status']) 

 

if __name__ == "__main__": 

    sendSMS()

If OTP==typed otp ;

       Continue;

Else;

     

 Print (" Enter correct otp")

Print ("login Successfully")

Do 

Copy_address=landlords_address 

#by using string indexing allow small changes

Validation_date=int(input("enter Validation date"))

If current_date<=Validation_date ;

  #Message to acceptor 

  Print("you need to change your address ")

Else;

  Continue;

Print("address ubdation done successfully ")

#code to send softcopy to fullfill current recruitment 

Print("you willget hard copy soon")

 
