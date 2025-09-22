# Search Completion System  

## Purpose of the program
The program is designed to provide users with an ability to get search term suggestions based on their input. The user can type a word or phrase, and the program will generate multiple possible suggestions and allow users to select one from a numbered list.

## What are the benefits of this program?
- It saves time by providing instant suggestions.
- It enhances user experience by making search more interactive.
- It helps users who may be unsure of what to type next.
- It leverages advanced language models to generate relevant completions.
- It can be adapted for various applications and platforms. For example, it could be integrated into a website or app to improve search functionality.
  
## How to run it  
1. Install Python(newer version).  
2. Install the Transformers library:  
   ```bash
   pip install transformers
3. Run the script:  
   ```bash
   python assignment04_chi_diep.py
   
## How the program works  
The program runs in five main steps:  

1. **Create a pipeline** → initializes a Hugging Face pipeline with the distilgpt2 model for text generation.  
2. **Ask for input** → prompts the user to type a word or phrase they want suggestions for.  
3. **Generate suggestions** → uses the model to generate 5 short completions (limited by max_length=7, so each suggestion is concise).  
4. **Show results** → displays the generated suggestions in a clear, numbered list.  
5. **Pick one** → allows the user to select a suggestion by number, and the program confirms their choice or asks them to choose again if it is out of range.

That's it! You can try it out!


