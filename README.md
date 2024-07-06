# tkinter
# The application uses the tkinter library to create and manage the GUI elements and the messagebox module to display the greeting message.

import tkinter as tk
from tkinter import messagebox

# Function to handle button click
def on_button_click():
    user_input = entry.get()
    messagebox.showinfo("Message", f"Hello, {user_input}!")

# Create main window
root = tk.Tk()
root.title("Simple GUI App")

# Create label
label = tk.Label(root, text="Enter your name:")
label.pack(pady=10)

# Create entry widget
entry = tk.Entry(root)
entry.pack(pady=10)

# Create button
button = tk.Button(root, text="Say Hello", command=on_button_click)
button.pack(pady=10)

# Run the main loop
root.mainloop()
