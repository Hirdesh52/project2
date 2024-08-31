# project2
Word Counter (Build a program that counts the number of words in a given text)
def count_words(text):
    """
    This function takes a string as input and returns the number of words.
    """
    words = text.split()  # Split the text into words
    return len(words)  # Return the number of words

def main():
    # Prompt the user for input
    user_input = input("Please enter a sentence or paragraph: ")
    
    # Error handling for empty input
    if not user_input.strip():
        print("Error: The input cannot be empty. Please enter some text.")
    else:
        # Count the words
        word_count = count_words(user_input)
        
        # Display the word count
        print(f"The number of words in the text is: {word_count}")

# Run the main function
if __name__ == "__main__":
    main()
