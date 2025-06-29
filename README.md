def read_file(filename):
    try:
        with open(filename, 'r') as file:
            content = file.read()
            print("File content:\n", content)
    except FileNotFoundError:
        print("Error: The file was not found.")
    except PermissionError:
        print("Error: You don't have permission to read the file.")
    except Exception as e:
        print("An unexpected error occurred:", str(e))

# Example
file_name = input("Enter the filename: ")
read_file(file_name)



def write_to_file(filename, data):
    try:
        with open(filename, 'w') as file:
            file.write(data)
        print("Data written successfully.")
    except Exception as e:
        print("Error while writing to file:", str(e))

# Example
write_to_file("example.txt", "This is the first line.\n")


def append_to_file(filename, data):
    try:
        with open(filename, 'a') as file:
            file.write(data)
        print("Data appended successfully.")
    except Exception as e:
        print("Error while appending to file:", str(e))

# Example
append_to_file("example.txt", "This is an additional line.\n")


    
