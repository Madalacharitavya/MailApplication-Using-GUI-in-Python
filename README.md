This code creates a simple email sender application using the `smtplib` library for sending emails and Tkinter for the graphical user interface (GUI).

1. Importing necessary modules:
   - `import smtplib` imports the `smtplib` module, which is used for sending emails using the Simple Mail Transfer Protocol (SMTP).
   - `from tkinter import *` imports all the classes, functions, and constants from the Tkinter module.
2. Function definition:
   - `send_message()`: This function is called when the "Send Message" button is clicked. It retrieves the values entered in the GUI fields (sender's email, password, recipient's email, and email body) using the `get()` method on the respective `StringVar` objects.
   - It creates an SMTP server instance with the Gmail SMTP server address and port (smtp.gmail.com:587).
   - It initiates a secure TLS connection using `starttls()` to encrypt the communication with the server.
   - It logs in to the SMTP server using the sender's email and password provided.
   - It sends the email by calling `sendmail()` on the SMTP server instance with the sender's email, recipient's email, and email body as arguments.
   - Finally, it clears the GUI input fields using `delete()` on the respective `Entry` widgets.
3.Creating the GUI:
   - An instance of `Tk()` is created and assigned to the variable `gui`.
   - The window dimensions are set using `gui.geometry("500x500")`.
   - The title of the GUI window is set using `gui.title("Email Sender App")`.
   - The background color of the GUI is set to light blue using `gui.configure(background="light blue")`.
4. Creating and placing GUI widgets:
   - The heading label is created using `Label()` with text, background color, foreground color, font, width, and height parameters. It is then packed using `pack()`.
   - Labels, entry fields, and the button are created using `Label()` and `Entry()`, specifying the respective text variable (`StringVar`) and width. They are placed in the GUI window using `place()`.
   - The button is created using `Button()` with text, command, width, height, and background color parameters. It is placed using `place()`.
5. Running the GUI:
   - The `mainloop()` function is called to start the Tkinter event loop, which keeps the GUI window open and handles user interactions.
When the user fills in the required fields and clicks the "Send Message" button, the `send_message()` function is triggered, establishing a connection to the SMTP server, logging in, and sending the email.

https://github.com/Madalacharitavya/MailApplication-Using-GUI-in-Python/assets/102969979/067321df-da3a-4d35-b5af-914799d37ab0



