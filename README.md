
# Cover Letter Generator Using OpenAI's GPT-3.5 API

This program is designed to automatically generate cover letters for multiple job advertisements using the OpenAI GPT-3.5 API. It reads your resume from a text file, and for each job advertisement, it creates a personalized cover letter referencing your resume and saves it as a separate text file.

Copied from [Ben-J-Orr](https://github.com/Ben-J-Orr/CoverLetter-Generator.git)

![Screenshot](https://i.gyazo.com/8cf3c0f2132d604a0aae9498246bc96d.png)

## Key Features

- **Resume Input**: The program reads your resume from a plain text file, ensuring that it is easy to update and maintain. This allows the AI model to reference your resume when generating cover letters.
- **Multiple Job Advertisements**: The program supports generating cover letters for multiple job advertisements at once. Simply add your job advertisement text files to the designated folder, and the program will process each one sequentially.
- **OpenAI GPT-3.5 API**: The program uses the advanced GPT-3.5-turbo AI model from OpenAI to generate high-quality, personalized cover letters that reference both your resume and the specific job advertisement.
- **Cover Letter Output**: The generated cover letters are saved as separate text files in a designated output folder, making it easy to access, review, and submit them for job applications.
- **JSON Config**: Grab your OpenAI API key and additional promt parameters from a JSON file. 

## Prerequisites

An OpenAI API key is required to use this program. Visit https://beta.openai.com/signup/ to sign up for an API key if you don't have one already.

Ensure you have Python 3.6 or later installed on your system.

Install the openai Python package by running:
```bash
pip install openai
```
## Setup

- Clone the repository or download the source code.
- Create a config.json file in the root directory of the project with the following content:
```json
{
  "api-key": "your_openai_api_key",
  "additional_prompt_options": "optional_additional_prompt_options"
}
```
- Replace * *"your_openai_api_key"* * with your actual OpenAI API key and * *optional_additional_prompt_options* * with any additional options you'd like to include in the prompt  (e.g., specific instructions or constraints).
- Create a folder named resume in the same directory as the source code and add a text file named experience.txt containing your resume. Ensure the text file is UTF-8 encoded.
- Create a folder named Adverts in the same directory as the source code and add job advertisement text files you want to generate cover letters for.
- Create a folder named outputs in the same directory as the source code. This is where the generated cover letters will be saved.


## Usage

- Open a terminal/command prompt and navigate to the directory containing the source code.
- Run the program using:
  ```bash
  python main.py
  ```
- The program will display the current job advertisement being processed and generate cover letters for each job advertisement.
- Upon completion, the generated cover letters will be saved in the outputs folder, with filenames corresponding to the respective job advertisement filenames and an _Output.txt suffix.
- You can now view and use the generated cover letters for your job applications.

## Known Issues

The GPT-3.5 API accepts plain text input and might not interpret formatting elements as expected. Bullet points, special characters, or other formatting elements might be misinterpreted, resulting in an incorrect understanding of your resume and a less effective cover letter.

To avoid these issues, consider converting your resume into plain text before using it with this program. Remove any special characters or formatting elements and use plain text to represent your experience, skills, and other relevant information.

Keep in mind that the simpler and cleaner your resume is, the better the AI model will understand it and generate more effective cover letters.

## Acknowledgements

 - [OpenAI](https://github.com/openai/openai-python)
 - [ChatGPT](https://openai.com/blog/chatgpt)

![Logo](https://i.imgur.com/BBhcHDx.gif)


## License

[MIT](https://choosealicense.com/licenses/mit/)


