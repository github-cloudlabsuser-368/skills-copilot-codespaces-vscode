file_path = "/path/to/file.txt"

try:
    # Open the file in read mode
    file = open(file_path, "r")

    # Read the file contents
    file_contents = file.read()

    # Close the file
    file.close()

    # Do something with the file contents
    print(file_contents)

except FileNotFoundError:
    print("File not found.")

except IOError:
    print("Error reading the file.")