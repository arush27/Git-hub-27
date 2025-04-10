def read_file(Sample.txt):
     """
     
     """
     try:
         with open(Sample.txt, 'r') as file:
             for line in file:
                 print(line.strip())  # Print each line without leading/trailing spaces
     except FileNotFoundError:
         print(f"Error: The file '{file_path}' was not found.")
     except Exception as e:
         print(f"An unexpected error occurred: {e}")
 
 
 def write_and_append_to_file():
     filename = "output.txt"
     user_input = input("Enter some text to save to the file: ")
     with open(output.txt, "a") as file:
         file.write(user_input + "\n")
         print("\nContents of the file after writing:")
     with open(output.txt, "r") as file:
         contents = file.read()
         print(contents)
 
 
 write_and_append_to_file()
