# CYLEXA AI ASSISTANT

<!-- markdownlint-disable -->
<pre>
 $$$$$$\$$\     $$\$$\      $$$$$$$$\$$\   $$\ $$$$$$\         $$$$$$\ $$$$$$\        $$$$$$\  $$$$$$\  $$$$$$\ $$$$$$\ $$$$$$\$$$$$$$$\ $$$$$$\ $$\   $$\$$$$$$$$\ 
$$  __$$\$$\   $$  $$ |     $$  _____$$ |  $$ $$  __$$\       $$  __$$\\_$$  _|      $$  __$$\$$  __$$\$$  __$$\\_$$  _$$  __$$\__$$  __$$  __$$\$$$\  $$ \__$$  __|
$$ /  \__\$$\ $$  /$$ |     $$ |     \$$\ $$  $$ /  $$ |      $$ /  $$ | $$ |        $$ /  $$ $$ /  \__$$ /  \__| $$ | $$ /  \__| $$ |  $$ /  $$ $$$$\ $$ |  $$ |   
$$ |      \$$$$  / $$ |     $$$$$\    \$$$$  /$$$$$$$$ |      $$$$$$$$ | $$ |        $$$$$$$$ \$$$$$$\ \$$$$$$\   $$ | \$$$$$$\   $$ |  $$$$$$$$ $$ $$\$$ |  $$ |   
$$ |       \$$  /  $$ |     $$  __|   $$  $$< $$  __$$ |      $$  __$$ | $$ |        $$  __$$ |\____$$\ \____$$\  $$ |  \____$$\  $$ |  $$  __$$ $$ \$$$$ |  $$ |   
$$ |  $$\   $$ |   $$ |     $$ |     $$  /\$$\$$ |  $$ |      $$ |  $$ | $$ |        $$ |  $$ $$\   $$ $$\   $$ | $$ | $$\   $$ | $$ |  $$ |  $$ $$ |\$$$ |  $$ |   
\$$$$$$  |  $$ |   $$$$$$$$\$$$$$$$$\$$ /  $$ $$ |  $$ |      $$ |  $$ $$$$$$\       $$ |  $$ \$$$$$$  \$$$$$$  $$$$$$\\$$$$$$  | $$ |  $$ |  $$ $$ | \$$ |  $$ |   
 \______/   \__|   \________\________\__|  \__\__|  \__|      \__|  \__\______|      \__|  \__|\______/ \______/\______|\______/  \__|  \__|  \__\__|  \__|  \__|   
</pre>
<!-- markdownlint-enable -->



CYLEXA AI  Assistant is a versatile virtual assistant built by me, it is a python based program that can perform various tasks and provide real-time information. It uses OpenAI's GPT-3.5 language model to generate responses based on user input, enabling natural language conversations. With speech recognition and text-to-speech capabilities, the assistant can interact with the user through voice commands and responses. Whether you need to study,  play music, search and play YouTube videos, set reminders, list your reminders, open your web browser  or perform web searches directly through word of command, CYLEXA AI  Assistant is here to help.

## Installation and Setup
NB: still at it's early stages, works best on windows systems for now, might need additional audio input configurations on linux systems.

1. Clone the repository to your local machine using the following command:
   >git clone https://github.com/cy-cus/CYLEXA.git

2. Navigate to the project directory:
   >cd CYLEXA

3. (Optional) It is recommended to create a virtual environment to isolate the project's dependencies. You can use `venv`, `conda`, or any other preferred virtual environment tool.

4. Install the required dependencies by running:
   >pip install -r requirements.txt
   
5. Set up an OpenAI API key:
   >Sign up for an OpenAI account and obtain an API key.
 
   >Update the 'config.ini' file that is in the same directory as the cylexa.py with your API key where it is written "open_ai_api_key".

6. Run the application.
   > python3 cylexa.py

## Functionality

CYLEXA AI Assistant provides the following functionality:

1. Speech Recognition and Text-to-Speech:

    The assistant can listen to user input through the microphone using the speech_recognition library.
	It converts the user's speech to text and processes it.

2. Natural Language Processing:

   The assistant uses OpenAI's GPT-3.5 language model to generate responses based on user input.
   It sends the user's input to the model and receives a response.

3. Music Playback:

	The assistant can play music on YouTube.
	When the user asks to play music, the assistant listens for the song name, performs speech recognition, and plays the song using the pywhatkit library.
	
4. YouTube Video Playback:

	The assistant can search and play YouTube videos.
	When the user asks to search and play a YouTube video, the assistant listens for the video name, performs speech recognition, and plays the video using the pywhatkit library.
	
5. Web Search:

	The assistant can perform web searches on YouTube and Google.
	When the user asks to search on YouTube, the assistant extracts the search query from the user input and opens the YouTube search results in the default web browser.
	Similarly, when the user asks to search on Google, the assistant extracts the search query from the user input and opens the Google search results in the default web browser.
	
6. Reminders:

	The assistant can set reminders for the user.
	When the user asks to set a reminder, the assistant prompts the user for the reminder name, date due, and description.
	It stores the reminder information in a JSON file.
	
7. Reminder Inquiry:

	The assistant can list all the user's reminders.
	When the user asks to inquire about their reminders, the assistant retrieves the reminder information from the JSON file and reads it aloud.
	
8. System Operations:

	The assistant can perform system operations such as restarting the computer and listing running processes.
	When the user asks to restart the computer, the assistant restarts the computer using the subprocess library.
	Similarly, when the user asks to list running processes, the assistant retrieves the process information using the subprocess library and reads it aloud.




## Usage Example

Here's an example interaction with the CYLEXA AI Assistant:

User: "Hey CYLEXA, which one is the tallest mountain in the world."

Cylexa: "Mount Everest is the tallest mountain in the world, standing at a height of 8,848 meters (29,029 feet)."

User: "Hey CYLEXA, play some music."

Cylexa: "Sure, what song would you like to listen to?"

User: "Play 'Shape of You' by Ed Sheeran."

Cylexa: Plays the song 'Shape of You' by Ed Sheeran on YouTube.

User: "Search YouTube for 'funny cat videos'."

Cylexa: Opens the YouTube search results for 'funny cat videos' in the default web browser.

User: "Set a reminder."

Cylexa: "Sure, what should I remind you of?"

User: "Reminder: Call John tomorrow at 3 p.m."

Cylexa: "Got it. I will remind you to 'Call John tomorrow at 3 p.m.'"

User: "Inquire reminders."

Cylexa: Reads aloud the list of reminders: "You have a reminder to Call John tomorrow at 3 p.m."

User: "Exit CYLEXA."

Cylexa: "Goodbye! Have a great day!"




## Limitations

While the CYLEXA AI Assistant is capable of performing various tasks and providing real-time information, there are some limitations to keep in mind:

1.Dependency on Internet Connection:

The assistant requires an active internet connection to interact with the OpenAI API, play YouTube videos, and perform web searches.

2. OpenAI API Limits:

The assistant is limited by the API usage limits of OpenAI. Exceeding these limits may result in rate limiting or additional charges, depending on your OpenAI subscription.

3.Accuracy of Speech Recognition:

The accuracy of speech recognition may vary depending on the user's microphone and the clarity of their speech.
	
4. Restricted Access:

The assistant can only access information available on the internet or provided through the OpenAI API. It cannot access personal files, passwords, or private information.

5. System Operations Limitations:

System operations such as restarting the computer may require appropriate permissions, and the availability of certain operations may depend on the user's operating system and configuration




CYLEXA AI Assistant is constantly learning and evolving. We welcome all suggestions, improvements, and ideas to enhance its capabilities. Help us make CYLEXA even better by providing your valuable input. Together, let's use artificial intelligence for the best!
