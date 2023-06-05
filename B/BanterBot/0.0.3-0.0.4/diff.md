# Comparing `tmp/BanterBot-0.0.3.tar.gz` & `tmp/BanterBot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BanterBot-0.0.3.tar", last modified: Thu Jun  1 22:53:33 2023, max compression
+gzip compressed data, was "BanterBot-0.0.4.tar", last modified: Mon Jun  5 21:51:08 2023, max compression
```

## Comparing `BanterBot-0.0.3.tar` & `BanterBot-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.681945 BanterBot-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.597945 BanterBot-0.0.3/BanterBot.egg-info/
--rw-rw-rw-   0        0        0     5220 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1169 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 22:53:33.000000 BanterBot-0.0.3/BanterBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5220 2023-06-01 22:53:33.682445 BanterBot-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4115 2023-06-01 22:52:41.000000 BanterBot-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.598945 BanterBot-0.0.3/banterbot/
--rw-rw-rw-   0        0        0      645 2023-05-30 22:17:56.000000 BanterBot-0.0.3/banterbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.610444 BanterBot-0.0.3/banterbot/core/
--rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.3/banterbot/core/__init__.py
--rw-rw-rw-   0        0        0     7373 2023-05-31 21:07:43.000000 BanterBot-0.0.3/banterbot/core/openai_manager.py
--rw-rw-rw-   0        0        0     6355 2023-06-01 22:30:44.000000 BanterBot-0.0.3/banterbot/core/speech_to_text.py
--rw-rw-rw-   0        0        0    12535 2023-06-01 22:30:45.000000 BanterBot-0.0.3/banterbot/core/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.621445 BanterBot-0.0.3/banterbot/data/
--rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/data/__init__.py
--rw-rw-rw-   0        0        0     7198 2023-05-31 21:31:32.000000 BanterBot-0.0.3/banterbot/data/azure_neural_voices.py
--rw-rw-rw-   0        0        0      455 2023-05-30 21:54:12.000000 BanterBot-0.0.3/banterbot/data/config.py
--rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.3/banterbot/data/enums.py
--rw-rw-rw-   0        0        0     2981 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/data/openai_models.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.635945 BanterBot-0.0.3/banterbot/gui/
--rw-rw-rw-   0        0        0      185 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/gui/__init__.py
--rw-rw-rw-   0        0        0     8550 2023-06-01 21:50:45.000000 BanterBot-0.0.3/banterbot/gui/banter_bot_interface.py
--rw-rw-rw-   0        0        0     7048 2023-06-01 22:30:45.000000 BanterBot-0.0.3/banterbot/gui/banter_bot_tk.py
--rw-rw-rw-   0        0        0     1911 2023-06-01 22:49:44.000000 BanterBot-0.0.3/banterbot/gui/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.657945 BanterBot-0.0.3/banterbot/utils/
--rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.3/banterbot/utils/__init__.py
--rw-rw-rw-   0        0        0     3270 2023-05-31 21:31:32.000000 BanterBot-0.0.3/banterbot/utils/message.py
--rw-rw-rw-   0        0        0     5725 2023-05-31 21:25:27.000000 BanterBot-0.0.3/banterbot/utils/nlp.py
--rw-rw-rw-   0        0        0     7633 2023-05-31 22:27:47.000000 BanterBot-0.0.3/banterbot/utils/speech_to_text_output.py
--rw-rw-rw-   0        0        0     3887 2023-05-30 21:54:12.000000 BanterBot-0.0.3/banterbot/utils/text_to_speech_output.py
--rw-rw-rw-   0        0        0     2895 2023-05-28 15:33:48.000000 BanterBot-0.0.3/banterbot/utils/thread_queue.py
--rw-rw-rw-   0        0        0     3097 2023-05-31 22:01:51.000000 BanterBot-0.0.3/banterbot/utils/word.py
--rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      133 2023-06-01 22:53:33.683945 BanterBot-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2214 2023-06-01 22:49:28.000000 BanterBot-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.659945 BanterBot-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.663945 BanterBot-0.0.3/tests/core/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/core/__init__.py
--rw-rw-rw-   0        0        0     8818 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/core/test_openai_manager.py
--rw-rw-rw-   0        0        0     2661 2023-06-01 22:30:45.000000 BanterBot-0.0.3/tests/core/test_text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:53:33.679945 BanterBot-0.0.3/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_message.py
--rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_nlp.py
--rw-rw-rw-   0        0        0     3087 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_text_to_speech_output.py
--rw-rw-rw-   0        0        0     1239 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_text_to_speech_word.py
--rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.3/tests/utils/test_thread_queue.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.947049 BanterBot-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.857545 BanterBot-0.0.4/BanterBot.egg-info/
+-rw-rw-rw-   0        0        0     6669 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 21:51:08.000000 BanterBot-0.0.4/BanterBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6669 2023-06-05 21:51:08.947049 BanterBot-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5564 2023-06-05 20:27:33.000000 BanterBot-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.858546 BanterBot-0.0.4/banterbot/
+-rw-rw-rw-   0        0        0      740 2023-06-05 20:28:59.000000 BanterBot-0.0.4/banterbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.871547 BanterBot-0.0.4/banterbot/core/
+-rw-rw-rw-   0        0        0      251 2023-05-30 22:17:56.000000 BanterBot-0.0.4/banterbot/core/__init__.py
+-rw-rw-rw-   0        0        0     8586 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/openai_manager.py
+-rw-rw-rw-   0        0        0     7671 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/speech_to_text.py
+-rw-rw-rw-   0        0        0    13493 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/core/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.883047 BanterBot-0.0.4/banterbot/data/
+-rw-rw-rw-   0        0        0      196 2023-05-29 12:59:46.000000 BanterBot-0.0.4/banterbot/data/__init__.py
+-rw-rw-rw-   0        0        0     7570 2023-06-04 19:42:55.000000 BanterBot-0.0.4/banterbot/data/azure_neural_voices.py
+-rw-rw-rw-   0        0        0      605 2023-06-04 19:49:08.000000 BanterBot-0.0.4/banterbot/data/config.py
+-rw-rw-rw-   0        0        0      660 2023-05-31 21:31:33.000000 BanterBot-0.0.4/banterbot/data/enums.py
+-rw-rw-rw-   0        0        0     3347 2023-06-04 19:42:55.000000 BanterBot-0.0.4/banterbot/data/openai_models.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.898048 BanterBot-0.0.4/banterbot/gui/
+-rw-rw-rw-   0        0        0      280 2023-06-05 20:28:59.000000 BanterBot-0.0.4/banterbot/gui/__init__.py
+-rw-rw-rw-   0        0        0     2626 2023-06-05 20:03:52.000000 BanterBot-0.0.4/banterbot/gui/cli.py
+-rw-rw-rw-   0        0        0    11034 2023-06-05 21:44:50.000000 BanterBot-0.0.4/banterbot/gui/interface.py
+-rw-rw-rw-   0        0        0     6443 2023-06-05 21:46:26.000000 BanterBot-0.0.4/banterbot/gui/tk_multiplayer_interface.py
+-rw-rw-rw-   0        0        0     7487 2023-06-05 21:47:39.000000 BanterBot-0.0.4/banterbot/gui/tk_simple_interface.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.924049 BanterBot-0.0.4/banterbot/utils/
+-rw-rw-rw-   0        0        0       67 2023-05-29 12:59:46.000000 BanterBot-0.0.4/banterbot/utils/__init__.py
+-rw-rw-rw-   0        0        0     3270 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/message.py
+-rw-rw-rw-   0        0        0     5723 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/nlp.py
+-rw-rw-rw-   0        0        0     7631 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/speech_to_text_output.py
+-rw-rw-rw-   0        0        0     3887 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/text_to_speech_output.py
+-rw-rw-rw-   0        0        0     2895 2023-06-04 19:42:56.000000 BanterBot-0.0.4/banterbot/utils/thread_queue.py
+-rw-rw-rw-   0        0        0     3095 2023-06-05 21:46:06.000000 BanterBot-0.0.4/banterbot/utils/word.py
+-rw-rw-rw-   0        0        0       93 2023-05-02 23:01:02.000000 BanterBot-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      133 2023-06-05 21:51:08.949549 BanterBot-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2216 2023-06-04 20:11:00.000000 BanterBot-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.926048 BanterBot-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.929548 BanterBot-0.0.4/tests/core/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     8816 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/core/test_openai_manager.py
+-rw-rw-rw-   0        0        0     2659 2023-06-05 21:46:07.000000 BanterBot-0.0.4/tests/core/test_text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:51:08.944550 BanterBot-0.0.4/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     1655 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_message.py
+-rw-rw-rw-   0        0        0     1362 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_nlp.py
+-rw-rw-rw-   0        0        0     3085 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/utils/test_text_to_speech_output.py
+-rw-rw-rw-   0        0        0     1237 2023-06-05 21:46:06.000000 BanterBot-0.0.4/tests/utils/test_text_to_speech_word.py
+-rw-rw-rw-   0        0        0     2250 2023-05-28 15:33:48.000000 BanterBot-0.0.4/tests/utils/test_thread_queue.py
```

### Comparing `BanterBot-0.0.3/BanterBot.egg-info/PKG-INFO` & `BanterBot-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: BanterBot
-Version: 0.0.3
-Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
-Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.3-alpha/BanterBot-0.0.3.tar.gz
-Author: Gabriel S. Cabrera
-Author-email: gabriel.sigurd.cabrera@gmail.com
-Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-
 # BanterBot
 
 BanterBot is a user-friendly chatbot application that leverages OpenAI models for generating context-aware responses, Azure Neural Voices for text-to-speech synthesis, and Azure speech-to-text recognition. The package offers a comprehensive toolkit for building chatbot applications with an intuitive interface and a suite of utilities.
 
 ## Features
 
 * Employs OpenAI models for generating context-sensitive responses
@@ -49,21 +29,25 @@
 ### TextToSpeech
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
 ### SpeechToText
 A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
 
-### BanterBotInterface
+### Interface
 
 An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area. Accepts both keyboard inputs and microphone voice inputs.
 
-### BanterBotTK
+### TKSimpleInterface
+
+A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and Interface, offering a seamless integration of chatbot functionality with an intuitive interface.
+
+### TKMultiplayerInterface (In Development)
 
-A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
+This GUI establishes a multiplayer conversation environment where up to nine users can interact with the chatbot simultaneously. The GUI includes a conversation history area and user panels with 'Listen' buttons to process user input. It also supports key bindings for user convenience.
 
 ## Installation
 
 ### Pip (Recommended)
 
 BanterBot is installable using the Python Package Index (PyPi):
 
@@ -81,30 +65,56 @@
 python -m pip install .
 ```
 
 ## Usage
 
 ### Launch with Command Line
 
-Start BanterBot by running the `banterbot` command in your terminal. Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+Start BanterBot by running the `banterbot` command in your terminal.
+
+Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+
+Add the `-s` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-s "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."`).
+
+Add the `-m` flag to activate the multiplayer interface.
 
 ### Launch with a Python script
 
-To use BanterBot in a script, create an instance of the `BanterBotTK` class and call the `run` method:
+To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
 
 ```python
-from banterbot import BanterBotTK, get_voice_by_name, get_model_by_name
+from banterbot import TKInterface, get_voice_by_name, get_model_by_name
 
 model = get_model_by_name("gpt-3.5-turbo")
 voice = get_voice_by_name("Aria")
+
 style = "chat"
+# Optional system prompt to set up a custom character prior to initializing BanterBot.
+system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+
+# The four arguments `model`, `voice`, `style`, and `system` are optional.
+interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system)
+interface.run()
+```
+
+For multiplayer, you can modify the above code slightly:
+
+```python
+from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name
+
+model = get_model_by_name("gpt-3.5-turbo")
+voice = get_voice_by_name("Aria")
+style = "chat"
+
+# Optional system prompt to set up a custom character prior to initializing BanterBot.
+system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
 
-# The three arguments `model`, `voice`, and `style` are optional.
-BBTK = BanterBotTK(model=model, voice=voice, style=style)
-BBTK.run()
+# The four arguments `model`, `voice`, `style`, and `system` are optional.
+interface = TKMultiplayerInterface(model=model, voice=voice, style=style, system=system)
+interface.run()
 ```
 
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
```

### Comparing `BanterBot-0.0.3/BanterBot.egg-info/SOURCES.txt` & `BanterBot-0.0.4/BanterBot.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 banterbot/core/text_to_speech.py
 banterbot/data/__init__.py
 banterbot/data/azure_neural_voices.py
 banterbot/data/config.py
 banterbot/data/enums.py
 banterbot/data/openai_models.py
 banterbot/gui/__init__.py
-banterbot/gui/banter_bot_interface.py
-banterbot/gui/banter_bot_tk.py
 banterbot/gui/cli.py
+banterbot/gui/interface.py
+banterbot/gui/tk_multiplayer_interface.py
+banterbot/gui/tk_simple_interface.py
 banterbot/utils/__init__.py
 banterbot/utils/message.py
 banterbot/utils/nlp.py
 banterbot/utils/speech_to_text_output.py
 banterbot/utils/text_to_speech_output.py
 banterbot/utils/thread_queue.py
 banterbot/utils/word.py
```

### Comparing `BanterBot-0.0.3/PKG-INFO` & `BanterBot-0.0.4/BanterBot.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: BanterBot
-Version: 0.0.3
+Version: 0.0.4
 Summary: BanterBot: An OpenAI ChatGPT-powered chatbot with Azure Neural Voices. Supports speech-to-text and text-to-speech interactions. Features real-time monitoring and Tkinter frontend.
 Home-page: https://github.com/GabrielSCabrera/BanterBot
-Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.3-alpha/BanterBot-0.0.3.tar.gz
+Download-URL: https://github.com/GabrielSCabrera/BanterBot/releases/download/v0.0.4-alpha/BanterBot-0.0.4.tar.gz
 Author: Gabriel S. Cabrera
 Author-email: gabriel.sigurd.cabrera@gmail.com
 Keywords: tkinter,tk,gpt,gui,windows,linux,cross-platform,chatgpt,text-to-speech,speech-to-text,tts,stt,chatbot,openai,interactive
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -49,21 +49,25 @@
 ### TextToSpeech
 
 A class that handles text-to-speech synthesis using Azure's Cognitive Services. It supports a wide range of output formats, voices, and speaking styles. The synthesized speech can be interrupted, and the progress can be monitored in real-time.
 
 ### SpeechToText
 A class that provides an interface to convert spoken language into written text using Azure Cognitive Services. It allows continuous speech recognition and provides real-time results as sentences are recognized.
 
-### BanterBotInterface
+### Interface
 
 An abstract base class for designing frontends for the BanterBot application. It provides a high-level interface for managing conversations with the bot, including sending messages, receiving responses, and updating the conversation area. Accepts both keyboard inputs and microphone voice inputs.
 
-### BanterBotTK
+### TKSimpleInterface
 
-A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and BanterBotInterface, offering a seamless integration of chatbot functionality with an intuitive interface.
+A graphical user interface (GUI) for a chatbot application that employs OpenAI models for generating responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text. The class inherits from both tkinter.Tk and Interface, offering a seamless integration of chatbot functionality with an intuitive interface.
+
+### TKMultiplayerInterface (In Development)
+
+This GUI establishes a multiplayer conversation environment where up to nine users can interact with the chatbot simultaneously. The GUI includes a conversation history area and user panels with 'Listen' buttons to process user input. It also supports key bindings for user convenience.
 
 ## Installation
 
 ### Pip (Recommended)
 
 BanterBot is installable using the Python Package Index (PyPi):
 
@@ -81,30 +85,56 @@
 python -m pip install .
 ```
 
 ## Usage
 
 ### Launch with Command Line
 
-Start BanterBot by running the `banterbot` command in your terminal. Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+Start BanterBot by running the `banterbot` command in your terminal.
+
+Add the `-g` flag to enable GPT-4 for better quality conversations; note that this will only work if you have GPT-4 API access, and is both significantly more costly and slower than the default GPT-3.5-Turbo.
+
+Add the `-s` flag followed by a string in quotes to set up a custom character prior to initialization (e.g., `-s "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."`).
+
+Add the `-m` flag to activate the multiplayer interface.
 
 ### Launch with a Python script
 
-To use BanterBot in a script, create an instance of the `BanterBotTK` class and call the `run` method:
+To use BanterBot in a script, create an instance of the `TKSimpleInterface` class and call the `run` method:
+
+```python
+from banterbot import TKInterface, get_voice_by_name, get_model_by_name
+
+model = get_model_by_name("gpt-3.5-turbo")
+voice = get_voice_by_name("Aria")
+
+style = "chat"
+# Optional system prompt to set up a custom character prior to initializing BanterBot.
+system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+
+# The four arguments `model`, `voice`, `style`, and `system` are optional.
+interface = TKSimpleInterface(model=model, voice=voice, style=style, system=system)
+interface.run()
+```
+
+For multiplayer, you can modify the above code slightly:
 
 ```python
-from banterbot import BanterBotTK, get_voice_by_name, get_model_by_name
+from banterbot import TKMultiplayerInterface, get_voice_by_name, get_model_by_name
 
 model = get_model_by_name("gpt-3.5-turbo")
 voice = get_voice_by_name("Aria")
 style = "chat"
 
-# The three arguments `model`, `voice`, and `style` are optional.
-BBTK = BanterBotTK(model=model, voice=voice, style=style)
-BBTK.run()
+# Optional system prompt to set up a custom character prior to initializing BanterBot.
+system = "You are Grendel the Quiz Troll, a charismatic troll who loves to host quiz shows."
+
+# The four arguments `model`, `voice`, `style`, and `system` are optional.
+interface = TKMultiplayerInterface(model=model, voice=voice, style=style, system=system)
+interface.run()
 ```
 
 ## Chat Logs
 
 Chat logs are saved in the `$HOME/Documents/BanterBot/Conversations/` directory as individual `.txt` files.
 
 ## Documentation
```

### Comparing `BanterBot-0.0.3/banterbot/core/openai_manager.py` & `BanterBot-0.0.4/banterbot/core/openai_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import logging
 import os
 import time
 from typing import Generator, Iterator, List, Union
 
 import openai
-
 from banterbot.data.config import RETRY_LIMIT
 from banterbot.data.enums import EnvVar
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.nlp import NLP
 
 # Set the OpenAI API key
@@ -29,72 +29,109 @@
         """
         Initializes an OpenAIManager instance for a specific model.
 
         Args:
             model (OpenAIModel): The OpenAI model to be used. This should be an instance of the OpenAIModel class, which
             contains information about the model, such as its name and maximum token limit.
         """
+        # The selected model that will be used in OpenAI ChatCompletion prompts.
         self._model = model
 
-    def _count_tokens(self, messages: List[Message]) -> int:
+        # Indicates whether the current instance of OpenAIManager is streaming.
+        self._streaming = False
+
+        # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
+        self._interrupt: int = time.perf_counter_ns()
+
+    def prompt(self, messages: List[Message], **kwargs) -> List[str]:
         """
-        Calculates the total number of tokens in the given messages.
+        Sends messages to the OpenAI ChatCompletion API and retrieves the response as a list of sentences.
 
         Args:
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
             contains the content and role (user or assistant) of the message.
 
+            **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
+            and frequency_penalty.
+
         Returns:
-            int: The total number of tokens in the messages. This is used to ensure that the generated response does not
-            exceed the model's maximum token limit.
+            List[str]: A list of sentences forming the response from the OpenAI API. This can be used to display
+            the generated response to the user or for further processing.
         """
-        num_tokens = 3
-
-        for message in messages:
-            num_tokens += message.count_tokens(self._model)
-
-        return num_tokens
+        response = self._request(messages=messages, stream=False, **kwargs)
+        return NLP.segment_sentences(response)
 
-    def _response_parse_stream(self, response: Iterator) -> Generator[List[str], None, bool]:
+    def prompt_stream(self, messages: List[Message], **kwargs) -> Generator[List[str], None, None]:
         """
-        Parses a streaming response from the OpenAI API and yields blocks of text as they are received.
+        Sends messages to the OpenAI API and retrieves the response as a stream of blocks of sentences.
 
         Args:
-            response (Iterator): The streaming response object. This is the raw response received from the OpenAI API
-            when requesting a streaming response.
+            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
+            contains the content and role (user or assistant) of the message.
+
+            **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
+            and frequency_penalty.
 
         Yields:
-            Generator[List[str], None, bool]: Lists of sentences as blocks. Each block contains one or more sentences
-            that form a part of the generated response.
+            Generator[List[str], None, None]: A stream of blocks of sentences as the response from the OpenAI API. Each
+            block contains one or more sentences that form a part of the generated response. This can be used to display
+            the response to the user in real-time or for further processing.
+        """
+        # Record the time at which the request was made, in order to account for future interruptions.
+        init_time = time.perf_counter_ns()
 
-        Returns:
-            bool: True if the generator completed its iterations, False otherwise (due to interruption).
+        # Obtain a response from the OpenAI ChatCompletion API
+        response = self._request(messages=messages, stream=True, **kwargs)
+
+        # Set the streaming flag to True
+        self._streaming = True
+
+        # Yield the responses as they are streamed
+        for block in self._response_parse_stream(response=response, init_time=init_time):
+            yield block
+
+        # Reset the streaming flag to False
+        self._streaming = False
+
+    def interrupt(self) -> None:
         """
-        self._interrupt = False
-        text = ""
+        Interrupts any ongoing streaming processes. This method sets the interrupt flag to the current time, which will
+        cause any streaming processes activated prior to the current time to stop.
+        """
+        self._interrupt: int = time.perf_counter_ns()
+        logging.debug("interrupted OpenAIManager")
 
-        for chunk in response:
-            delta = chunk["choices"][0]["delta"]
+    @property
+    def streaming(self) -> bool:
+        """
+        If the current instance of OpenAIManager is in the process of streaming, returns True. Otherwise, returns False.
 
-            if self._interrupt:
-                return False
+        Args:
+            bool: The streaming state of the current instance.
+        """
+        return self._streaming
 
-            if "content" in delta.keys():
-                text += delta["content"]
+    def _count_tokens(self, messages: List[Message]) -> int:
+        """
+        Calculates the total number of tokens in the given messages.
 
-            if len(sentences := NLP.segment_sentences(text)) > 1:
-                text = sentences[-1]
-                yield sentences[:-1]
+        Args:
+            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
+            contains the content and role (user or assistant) of the message.
 
-            time.sleep(0.005)
+        Returns:
+            int: The total number of tokens in the messages. This is used to ensure that the generated response does not
+            exceed the model's maximum token limit.
+        """
+        num_tokens = 3
 
-        sentences = NLP.segment_sentences(text)
-        yield sentences
+        for message in messages:
+            num_tokens += message.count_tokens(self._model)
 
-        return True
+        return num_tokens
 
     def _request(self, messages: List[Message], stream: bool, **kwargs) -> Union[Iterator, str]:
         """
         Sends a request to the OpenAI API and generates a response based on the given parameters.
 
         Args:
             messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
@@ -124,53 +161,43 @@
                 time.sleep(0.25)
 
         if not success:
             raise openai.error.APIError
 
         return response if stream else response.choices[0].message.content.strip()
 
-    def interrupt(self) -> None:
-        """
-        Sets the interruption flag to True, which will stop the streaming response. This can be used to manually
-        interrupt the streaming response if needed, for example, if the user sends a new message before the current
-        response is completed.
-        """
-        self._interrupt = True
-
-    def prompt(self, messages: List[Message], **kwargs) -> List[str]:
+    def _response_parse_stream(self, response: Iterator, init_time: int) -> Generator[List[str], None, bool]:
         """
-        Sends messages to the OpenAI API and retrieves the response as a list of sentences.
+        Parses a streaming response from the OpenAI API and yields blocks of text as they are received.
 
         Args:
-            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
-            contains the content and role (user or assistant) of the message.
+            response (Iterator): A streaming response from the OpenAI ChatCompletion API.
+            init_time (int): The time at which the stream was initialized.
 
-            **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
-            and frequency_penalty.
+        Yields:
+            Generator[List[str], None, bool]: Lists of sentences as blocks. Each block contains one or more sentences
+            that form a part of the generated response.
 
         Returns:
-            List[str]: A list of sentences forming the response from the OpenAI API. This can be used to display
-            the generated response to the user or for further processing.
+            bool: True if the generator completed its iterations, False otherwise (due to interruption).
         """
-        response = self._request(messages=messages, stream=False, **kwargs)
-        return NLP.segment_sentences(response)
+        text = ""
+        logging.debug("streaming started")
 
-    def prompt_stream(self, messages: List[Message], **kwargs) -> Generator[List[str], None, None]:
-        """
-        Sends messages to the OpenAI API and retrieves the response as a stream of blocks of sentences.
+        for chunk in response:
+            delta = chunk["choices"][0]["delta"]
 
-        Args:
-            messages (List[Message]): A list of messages. Each message should be an instance of the Message class, which
-            contains the content and role (user or assistant) of the message.
+            if self._interrupt >= init_time:
+                return False
 
-            **kwargs: Additional parameters for the API request. These can include settings such as temperature, top_p,
-            and frequency_penalty.
+            if "content" in delta.keys():
+                text += delta["content"]
 
-        Yields:
-            Generator[List[str], None, None]: A stream of blocks of sentences as the response from the OpenAI API. Each
-            block contains one or more sentences that form a part of the generated response. This can be used to display
-            the response to the user in real-time or for further processing.
-        """
-        response = self._request(messages=messages, stream=True, **kwargs)
+            if len(sentences := NLP.segment_sentences(text)) > 1:
+                text = sentences[-1]
+                yield sentences[:-1]
 
-        for block in self._response_parse_stream(response=response):
-            yield block
+        sentences = NLP.segment_sentences(text)
+        yield sentences
+
+        logging.debug("streaming stopped")
+        return True
```

### Comparing `BanterBot-0.0.3/banterbot/core/speech_to_text.py` & `BanterBot-0.0.4/banterbot/core/speech_to_text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import logging
 import os
 import threading
+import time
 from typing import Generator, List
 
 import azure.cognitiveservices.speech as speechsdk
-
 from banterbot.data.enums import EnvVar
 from banterbot.utils.speech_to_text_output import SpeechToTextOutput
 from banterbot.utils.word import Word
 
 
 class SpeechToText:
     """
@@ -47,34 +48,81 @@
 
         # Creating a new instance of Connection class
         self._connection = speechsdk.Connection.from_recognizer(self._recognizer)
 
         # Preconnecting the speech recognizer for reduced latency
         self._connection.open(True)
 
+        # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
+        self._interrupt: int = time.perf_counter_ns()
+
         # Reset the state variables of the speech-to-text recognizer
         self._reset()
 
     def interrupt(self) -> None:
         """
-        Interrupts an ongoing speech-to-text process, if any. This method sets the interrupt flag, which will cause the
-        ongoing speech-to-text process to stop.
+        Interrupts an ongoing speech-to-text process, if any. This method sets the interrupt flag to the current time,
+        which will cause any speech-to-text processes activated prior to the current time to stop.
+        """
+        # Update the interruption time.
+        self._interrupt: int = time.perf_counter_ns()
+        # Release the threading.Event instance that the listener is waiting for.
+        self._new_events.set()
+        logging.debug("interrupted SpeechToText")
+
+    def listen(self) -> Generator[str, None, None]:
         """
-        self._interrupt = True
+        Starts the speech-to-text recognition process and yields sentences as they are recognized.
+
+        Yields:
+            Generator[str, None, None]: A generator that yields tuples of recognized sentences.
+        """
+        # Record the time at which the thread was initialized pre-lock, in order to account for future interruptions.
+        init_time = time.perf_counter_ns()
+
+        # Only allow one listener to be active at once.
+        with self.__class__._listen_lock:
+
+            # Do not run the listener if an interruption was raised after `init_time`.
+            if self._interrupt < init_time:
+
+                # Prepare a list which will contain all the recognized input words.
+                output = []
+                self._outputs.append(output)
+
+                # Set the listening flag to True
+                self._listening = True
+
+                # Starting the speech recognizer
+                self._recognizer.start_continuous_recognition()
+
+                # Monitor the recognition progress in the main thread, yielding sentences as they are processed
+                for block in self._process_callbacks(output, init_time):
+                    yield block
+
+                # Reset all state attributes
+                self._reset()
+
+    @property
+    def listening(self) -> bool:
+        """
+        If the current instance of SpeechToText is in the process of listening, returns True. Otherwise, returns False.
+
+        Args:
+            bool: The listening state of the current instance.
+        """
+        return self._listening
 
     def _reset(self) -> None:
         """
-        Resets the state variables of the speech-to-text recognizer, such as the list of events, recognition started
-        flag, and interrupt flag.
+        Resets the state variables of the speech-to-text recognizer, such as the list of events, the listening flag,
+        recognition started flag, and new events flag.
         """
-        # Reset the list of events that have been processed
         self._events: List[SpeechToTextOutput] = []
-
-        # Reset the recognition threading.Event instance and set the interrupt flag to False
-        self._interrupt: bool = False
+        self._listening: bool = False
         self._start_recognition: threading.Event = threading.Event()
         self._new_events: threading.Event = threading.Event()
 
     def _recognizer_events_connect(self) -> None:
         """
         Connects the speech-to-text recognizer events to their corresponding callbacks.
         """
@@ -99,61 +147,42 @@
 
         Args:
             event (speechsdk.SpeechRecognitionEventArgs): The recognized speech event.
         """
         self._events.append(SpeechToTextOutput(event.result))
         self._new_events.set()
 
-    def _process_callbacks(self, output: List[SpeechToTextOutput]) -> Generator[str, None, None]:
+    def _process_callbacks(self, output: List[SpeechToTextOutput], init_time: int) -> Generator[str, None, None]:
         """
         Processes the recognized speech events and appends them to the output list. Yields sentences as they are
         processed.
 
         Args:
-            output (List[SpeechToTextOutput]): The list to store the recognized speech events.
+            output (List[SpeechToTextOutput]): The list in which to store the recognized speech events.
+            init_time (int): The time at which the listening was initialized.
 
         Yields:
             Generator[str, None, None]: A generator that yields sentences as they are processed.
         """
         # Initialize variables
-        word_index = 0
+        idx = 0
 
         # Wait until the recognition has started before proceeding
         self._start_recognition.wait()
 
+        logging.debug("listening started")
+
         # Continuously monitor the recognition progress
-        while not self._interrupt:
+        while self._interrupt < init_time:
 
             self._new_events.wait()
             self._new_events.clear()
 
-            while not self._interrupt and word_index < len(self._events):
-                event = self._events[word_index]
+            while self._interrupt < init_time and idx < len(self._events):
+                event = self._events[idx]
                 output.append(event)
-                word_index += 1
+                idx += 1
                 yield str(event)
 
         # Stop the recognizer
         self._recognizer.stop_continuous_recognition()
-
-    def listen(self) -> Generator[str, None, None]:
-        """
-        Starts the speech-to-text recognition process and yields sentences as they are recognized.
-
-        Yields:
-            Generator[str, None, None]: A generator that yields tuples of recognized sentences.
-        """
-        with self.__class__._listen_lock:
-
-            # Reset all state attributes
-            self._reset()
-
-            # Prepare a list which will contain all the recognized input words.
-            output = []
-            self._outputs.append(output)
-
-            # Starting the speech recognizer
-            self._recognizer.start_continuous_recognition()
-
-            # Continuously monitor the recognition progress in the main thread, yielding sentences as they are processed
-            for block in self._process_callbacks(output):
-                yield block
+        logging.debug("listening stopped")
```

### Comparing `BanterBot-0.0.3/banterbot/core/text_to_speech.py` & `BanterBot-0.0.4/banterbot/core/text_to_speech.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
+import logging
 import os
 import threading
 import time
 from typing import Generator, List, Optional, TypedDict
 
 import azure.cognitiveservices.speech as speechsdk
 from azure.cognitiveservices.speech import SpeechSynthesisOutputFormat
-
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import EnvVar, SpeechProcessingType, WordCategory
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 from banterbot.utils.word import Word
 
 
 class TimedEvent(TypedDict):
@@ -59,42 +59,103 @@
         # Initialize the speech synthesizer with the speech configuration
         self._synthesizer = speechsdk.SpeechSynthesizer(speech_config=self._speech_config)
 
         # Set the speech synthesis output format to the specified output format
         self._speech_config.set_speech_synthesis_output_format(output_format)
 
         # Connect the speech synthesizer events to their corresponding callbacks
-        self._synthesizer_events_connect()
+        self._callbacks_connect()
 
         # Creating a new instance of Connection class
         self._connection = speechsdk.Connection.from_speech_synthesizer(self._synthesizer)
 
         # Preconnecting the speech synthesizer for reduced latency
         self._connection.open(True)
 
+        # Set the interruption flag to the current time: if interruptions are raised, this will be updated.
+        self._interrupt: int = time.perf_counter_ns()
+
         # Reset the state variables of the text-to-speech synthesizer
         self._reset()
 
     @property
     def output(self) -> List[TextToSpeechOutput]:
         """
         Getter for the output property, which is a list of TextToSpeechOutput objects.
 
         Returns:
             List[TextToSpeechOutput]: The list of synthesized outputs.
         """
         return self._outputs
 
+    @property
+    def speaking(self) -> bool:
+        """
+        If the current instance of TextToSpeech is in the process of speaking, returns True. Otherwise, returns False.
+
+        Args:
+            bool: The speaking state of the current instance.
+        """
+        return self._speaking
+
     def interrupt(self) -> None:
         """
-        Interrupts an ongoing text-to-speech process, if any.
+        Interrupts an ongoing text-to-speech process, if any. This method sets the interrupt flag to the current time,
+        which will cause any text-to-speech processes activated prior to the current time to stop.
+        """
+        self._interrupt: int = time.perf_counter_ns()
+        logging.debug("interrupted TextToSpeech")
 
-        This method sets the interrupt flag, which will cause the ongoing text-to-speech process to stop.
+    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[Word, None, bool]:
         """
-        self._interrupt = True
+        Speaks the given text using the specified voice and style.
+
+        This method converts the input text into speech using the specified voice and style. It yields the synthesized
+        words one by one, along with their contextual information.
+
+        Args:
+            input_string (str): The input string that is to be converted into speech.
+            voice (AzureNeuralVoice): The voice to be used.
+            style (str): The speaking style to be applied.
+
+        Yields:
+            Word: A word with contextual information.
+        """
+        # Record the time at which the thread was initialized pre-lock, in order to account for future interruptions.
+        init_time = time.perf_counter_ns()
+
+        # Create SSML markup for the given input_string, voice, and style
+        ssml = self._create_ssml(input_string, voice, style)
+
+        # Create a new thread to handle the speech synthesis
+        speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
+
+        with self.__class__._speech_lock:
+
+            # Do not run the listener if an interruption was raised after `init_time`.
+            if self._interrupt < init_time:
+
+                # Prepare an instance of TextToSpeechOutput while will receive values iteratively
+                output = TextToSpeechOutput(
+                    input_string=input_string, timestamp=datetime.datetime.now(), voice=voice, style=style
+                )
+                self._outputs.append(output)
+
+                # Starting the speech synthesizer
+                speech_thread.start()
+
+                # Set the speaking flag to True
+                self._speaking = True
+
+                # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
+                for word in self._callbacks_process(output, init_time):
+                    yield word
+
+                # Reset all state attributes
+                self._reset()
 
     def _callback_completed(self, event: speechsdk.SessionEventArgs) -> None:
         """
         Callback function for synthesis completed event.
         Sets the synthesis completed flag to True.
 
         Args:
@@ -126,61 +187,15 @@
             self._events.append(
                 {
                     "event": event,
                     "time": 5e8 + 100 * event.audio_offset + 1e9 * event.duration.total_seconds() / event.word_length,
                 }
             )
 
-    def _create_ssml(self, text: str, voice: str, style: Optional[str] = None) -> str:
-        """
-        Creates an SSML string from the given text, voice, and style.
-
-        Args:
-            text (str): The input string that is to be converted into speech.
-            voice (AzureNeuralVoice): The voice to be used.
-            style (str, optional): The speaking style to be applied. Default is None.
-
-        Returns:
-            str: The SSML string.
-        """
-        # Start the SSML string with the required header and voice tag
-        ssml = (
-            '<speak version="1.0" '
-            'xmlns="http://www.w3.org/2001/10/synthesis" '
-            'xmlns:mstts="https://www.w3.org/2001/mstts" '
-            'xml:lang="en-US">'
-            f'<voice name="{voice.voice}">'
-        )
-
-        # If a speaking style is specified, add the express-as tag
-        if style:
-            text = f'<mstts:express-as style="{style}">{text}</mstts:express-as>'
-
-        # Add the text to the SSML string
-        ssml += text
-
-        # Close the voice and speak tags and return the SSML string
-        ssml += "</voice></speak>"
-        return ssml
-
-    def _reset(self) -> None:
-        """
-        Resets the state variables of the text-to-speech synthesizer, such as the list of events, synthesis timer,
-        synthesis started flag, synthesis completed flag, and interrupt flag.
-        """
-        # Reset the list of boundaries that have been processed
-        self._events: List[TimedEvent] = []
-
-        # Reset the synthesis threading.Event, set the start timer to None, and reset the interrupt & completed flags
-        self._interrupt = False
-        self._start_timer = None
-        self._synthesis_completed = False
-        self._start_synthesis = threading.Event()
-
-    def _synthesizer_events_connect(self) -> None:
+    def _callbacks_connect(self) -> None:
         """
         Connects the text-to-speech synthesizer events to their corresponding callbacks.
 
         This method connects the synthesis_started, synthesis_word_boundary, synthesis_canceled, and synthesis_completed
         events to their respective callback functions.
         """
         # Connect the synthesis_started event to the _callback_started method
@@ -189,121 +204,128 @@
         # Connect the synthesis_word_boundary event to the _callback_word_boundary method
         self._synthesizer.synthesis_word_boundary.connect(self._callback_word_boundary)
 
         # Connect the synthesis_canceled and synthesis_completed events to the _callback_completed method
         self._synthesizer.synthesis_canceled.connect(self._callback_completed)
         self._synthesizer.synthesis_completed.connect(self._callback_completed)
 
-    def _process_boundary(self, word_index: int) -> Word:
-        """
-        Processes a synthesis boundary event and returns an instance of class Word.
-
-        Args:
-            word_index (int): The index of the word relative to the full text.
-
-        Returns:
-            Word: The processed word with contextual information.
-        """
-        event = self._events[word_index]["event"]
-        whitespace = ""
-        if event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Word:
-            category = WordCategory.WORD
-            if word_index > 0:
-                whitespace = " "
-        elif event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Punctuation:
-            category = WordCategory.PUNCTUATION
-
-        word = Word(
-            word=whitespace + event.text,
-            offset=datetime.timedelta(microseconds=event.audio_offset / 10),
-            duration=event.duration,
-            category=category,
-            source=SpeechProcessingType.TTS,
-        )
-        return word
-
-    def _process_callbacks(self, output: TextToSpeechOutput) -> Generator[Word, None, bool]:
+    def _callbacks_process(self, output: TextToSpeechOutput, init_time: int) -> Generator[Word, None, bool]:
         """
         Monitors the synthesis progress and updates the output accordingly.
 
         This method continuously checks the synthesis progress and processes the boundaries. It updates the output
         object with the processed words and yields them one by one.
 
         Args:
             output (TextToSpeechOutput): The output object to which the processed words will be added.
+            init_time (int): The time at which the speech was initialized.
 
         Yields:
             Word: A word with contextual information.
 
         Returns:
             bool: True if the process completed successfully, False otherwise.
         """
         # Initialize variables
-        word_index = 0
+        idx = 0
         success = False
 
         # Wait until the synthesis has started before proceeding
         self._start_synthesis.wait()
-        self._start_timer = time.perf_counter_ns()
+        start_timer = time.perf_counter_ns()
+
+        logging.debug("speech started")
 
         # Continuously monitor the synthesis progress
-        while not self._interrupt and (not self._synthesis_completed or word_index < len(self._events)):
+        while self._interrupt < init_time and (not self._synthesis_completed or idx < len(self._events)):
 
-            dt = time.perf_counter_ns() - self._start_timer
+            dt = time.perf_counter_ns() - start_timer
 
-            while not self._interrupt and word_index < len(self._events) and dt >= self._events[word_index]["time"]:
-                word = self._process_boundary(word_index=word_index)
+            while self._interrupt < init_time and idx < len(self._events) and dt >= self._events[idx]["time"]:
+                word = self._process_boundary(idx=idx)
                 output.append(word)
-                word_index += 1
+                idx += 1
                 yield word
 
             # Wait for a short amount of time before checking the synthesis progress again
             time.sleep(0.005)
 
-        if not self._interrupt:
+        if self._interrupt >= init_time:
             success = True
 
         # Stop the synthesizer
         self._synthesizer.stop_speaking()
+        logging.debug("speech stopped")
         return success
 
-    def _speak(self, ssml: str) -> None:
-        self._synthesizer.speak_ssml(ssml)
-
-    def speak(self, input_string: str, voice: AzureNeuralVoice, style: str) -> Generator[Word, None, bool]:
+    def _create_ssml(self, text: str, voice: str, style: Optional[str] = None) -> str:
         """
-        Speaks the given text using the specified voice and style.
-
-        This method converts the input text into speech using the specified voice and style. It yields the synthesized
-        words one by one, along with their contextual information.
+        Creates an SSML string from the given text, voice, and style.
 
         Args:
-            input_string (str): The input string that is to be converted into speech.
+            text (str): The input string that is to be converted into speech.
             voice (AzureNeuralVoice): The voice to be used.
-            style (str): The speaking style to be applied.
+            style (str, optional): The speaking style to be applied. Default is None.
 
-        Yields:
-            Word: A word with contextual information.
+        Returns:
+            str: The SSML string.
         """
-        # Create SSML markup for the given input_string, voice, and style
-        ssml = self._create_ssml(input_string, voice, style)
+        # Start the SSML string with the required header and voice tag
+        ssml = (
+            '<speak version="1.0" '
+            'xmlns="http://www.w3.org/2001/10/synthesis" '
+            'xmlns:mstts="https://www.w3.org/2001/mstts" '
+            'xml:lang="en-US">'
+            f'<voice name="{voice.voice}">'
+        )
 
-        # Create a new thread to handle the speech synthesis
-        speech_thread = threading.Thread(target=self._speak, args=(ssml,), daemon=True)
+        # If a speaking style is specified, add the express-as tag
+        if style:
+            text = f'<mstts:express-as style="{style}">{text}</mstts:express-as>'
 
-        with self.__class__._speech_lock:
+        # Add the text to the SSML string
+        ssml += text
 
-            # Reset all state attributes
-            self._reset()
+        # Close the voice and speak tags and return the SSML string
+        ssml += "</voice></speak>"
+        return ssml
 
-            # Prepare an instance of TextToSpeechOutput while will receive values iteratively
-            output = TextToSpeechOutput(
-                input_string=input_string, timestamp=datetime.datetime.now(), voice=voice, style=style
-            )
-            self._outputs.append(output)
+    def _process_boundary(self, idx: int) -> Word:
+        """
+        Processes a synthesis boundary event and returns an instance of class Word.
 
-            # Starting the speech synthesizer
-            speech_thread.start()
+        Args:
+            idx (int): The index of the word relative to the full text.
 
-            # Continuously monitor the synthesis progress in the main thread, yielding words as they are uttered
-            for word in self._process_callbacks(output):
-                yield word
+        Returns:
+            Word: The processed word with contextual information.
+        """
+        event = self._events[idx]["event"]
+        whitespace = ""
+        if event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Word:
+            category = WordCategory.WORD
+            if idx > 0:
+                whitespace = " "
+        elif event.boundary_type == speechsdk.SpeechSynthesisBoundaryType.Punctuation:
+            category = WordCategory.PUNCTUATION
+
+        word = Word(
+            word=whitespace + event.text,
+            offset=datetime.timedelta(microseconds=event.audio_offset / 10),
+            duration=event.duration,
+            category=category,
+            source=SpeechProcessingType.TTS,
+        )
+        return word
+
+    def _reset(self) -> None:
+        """
+        Resets the state variables of the text-to-speech synthesizer, such as the list of events, synthesis timer, the
+        interrupt flag, the speaking flag, the synthesis completed flag, and synthesis started flag.
+        """
+        self._events: List[TimedEvent] = []
+        self._speaking = False
+        self._synthesis_completed = False
+        self._start_synthesis = threading.Event()
+
+    def _speak(self, ssml: str) -> None:
+        self._synthesizer.speak_ssml(ssml)
```

### Comparing `BanterBot-0.0.3/banterbot/data/azure_neural_voices.py` & `BanterBot-0.0.4/banterbot/data/azure_neural_voices.py`

 * *Files 7% similar despite different names*

```diff
@@ -226,14 +226,22 @@
 
     Returns:
         AzureNeuralVoice: The corresponding AzureNeuralVoice instance.
 
     Raises:
         KeyError: If the specified name is not found in the _neural_voices dictionary.
     """
+    if name not in _neural_voices.keys():
+        available_voices = ", ".join(f"`{name}`" for name in _neural_voices.keys())
+        error_message = (
+            f"BanterBot was unable to load a Microsoft Azure neural voice model with the name `{name}`, available "
+            f"voices are: {available_voices}."
+        )
+        raise KeyError(error_message)
+
     return _neural_voices[name]
 
 
 def get_voices_by_gender(gender: AzureNeuralVoiceGender) -> List[AzureNeuralVoice]:
     """
     Retrieve a list of AzureNeuralVoice instances with the specified gender.
```

### Comparing `BanterBot-0.0.3/banterbot/data/enums.py` & `BanterBot-0.0.4/banterbot/data/enums.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.3/banterbot/data/openai_models.py` & `BanterBot-0.0.4/banterbot/data/openai_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,8 +82,16 @@
 
     Returns:
         OpenAIModel: The corresponding OpenAIModel instance.
 
     Raises:
         KeyError: If the specified name is not found in the _openai_models dictionary.
     """
+    if name not in _openai_models.keys():
+        available_models = ", ".join(f"`{name}`" for name in _openai_models.keys())
+        error_message = (
+            f"BanterBot was unable to load an OpenAI ChatCompletion model with the name `{name}`, available models "
+            f"are: {available_models}."
+        )
+        raise KeyError(error_message)
+
     return _openai_models[name]
```

### Comparing `BanterBot-0.0.3/banterbot/gui/banter_bot_interface.py` & `BanterBot-0.0.4/banterbot/gui/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,175 @@
 import datetime
+import logging
 import threading
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
 from banterbot.core.openai_manager import OpenAIManager
 from banterbot.core.speech_to_text import SpeechToText
 from banterbot.core.text_to_speech import TextToSpeech
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
-from banterbot.data.config import chat_logs
+from banterbot.data.config import chat_logs, logging_level
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.thread_queue import ThreadQueue
 
+logging.basicConfig(format="Interface %(asctime)s - %(message)s", level=logging_level)
 
-class BanterBotInterface(ABC):
+
+class Interface(ABC):
     """
-    BanterBotInterface is an abstract base class for creating frontends for the BanterBot application. It provides a
-    high-level interface for managing conversation with the bot, including sending messages, receiving responses, and
-    updating the conversation area. The interface supports both text and speech-to-text input for user messages.
+    Interface is an abstract base class for creating frontends for the BanterBot application. It provides a high-level
+    interface for managing conversation with the bot, including sending messages, receiving responses, and updating the
+    conversation area. The interface supports both text and speech-to-text input for user messages.
     """
 
-    def __init__(self, model: OpenAIModel, voice: AzureNeuralVoice, style: str) -> None:
+    def __init__(self, model: OpenAIModel, voice: AzureNeuralVoice, style: str, system: Optional[str] = None) -> None:
         """
         Initialize the BanterBotInterface with the given model, voice, and style.
 
         Args:
             model (OpenAIModel): The OpenAI model to use for generating responses.
             voice (AzureNeuralVoice): The voice to use for text-to-speech synthesis.
             style (str): The speaking style to use for text-to-speech synthesis.
+            system (Optional[str]): An initialization prompt that can be used to set the scene.
         """
-        # Initialize OpenAI ChatCompletion, Azure Speech-to-Text, and Azure Text-to-Speech components
+        # Initialize OpenAI ChatCompletion, Azure Speech-to-Text, and Azure text-to-speech components
         self._openai_manager = OpenAIManager(model=model)
         self._speech_to_text = SpeechToText()
         self._text_to_speech = TextToSpeech()
 
         # Initialize message handling and conversation attributes
         self._messages: List[Message] = []
-        self._output_lock = threading.Lock()
         self._log_lock = threading.Lock()
         self._log_path = chat_logs / f"chat_{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}.txt"
-        self._response_thread = None
-        self._listening = False
+        self._listening_toggle = False
 
         # Initialize thread management components
         self._thread_queue = ThreadQueue()
 
-        # Initialize voice and style attributes
+        # Initialize model, voice, and style attributes
+        self._model = model
         self._voice = voice
         self._style = style
 
+        # Initialize the system message, if provided
+        self._system = system
+        if self._system is not None:
+            message_instance = Message(role="system", content=system)
+            self._messages.append(message_instance)
+
         # Initialize the subclass GUI
         self._init_gui()
 
-    @abstractmethod
-    def _init_gui(self) -> None:
+    @property
+    def listening(self) -> bool:
         """
-        Initialize the graphical user interface for the frontend.
-        This method should be implemented by subclasses to create the specific GUI components.
+        If the current instance of SpeechToText is in the process of listening, returns True. Otherwise, returns False.
+
+        Args:
+            bool: The listening state of the current instance.
         """
+        return self._speech_to_text._listening
 
-    @abstractmethod
-    def update_conversation_area(self, word: str) -> None:
+    @property
+    def speaking(self) -> bool:
         """
-        Update the conversation area with the given word, and add the word to the chat log.
-        This method should be implemented by subclasses to handle updating the specific GUI components.
+        If the current instance of TextToSpeech is in the process of speaking, returns True. Otherwise, returns False.
 
         Args:
-            word (str): The word to add to the conversation area.
+            bool: The speaking state of the current instance.
         """
-        self._append_to_chat_log(word)
+        return self._text_to_speech.speaking
 
     @property
-    def listening(self) -> bool:
-        return self._listening
+    def streaming(self) -> bool:
+        """
+        If the current instance of OpenAIManager is in the process of streaming, returns True. Otherwise, returns False.
+
+        Args:
+            bool: The streaming state of the current instance.
+        """
+        return self._openai_manager.streaming
 
-    def send_message(self, user_message: str, name: Optional[str] = None) -> None:
+    def send_message(self, message: str, role: str = "user", name: Optional[str] = None) -> None:
         """
         Send a message from the user to the conversation.
 
         Args:
-            user_message (str): The message content from the user.
+            message (str): The message content from the user.
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
-        message = Message(role="user", name=name, content=user_message)
-        text = f"{message.name.title() if message.name is not None else 'User'}: {user_message}\n\n"
-        self._messages.append(message)
+        message_instance = Message(role=role, name=name, content=message)
+        text = f"{message_instance.name.title() if message_instance.name is not None else 'User'}: {message}\n\n"
+        self._messages.append(message_instance)
         self.update_conversation_area(word=text)
 
-    def prompt(self, user_message: str, name: Optional[str] = None) -> None:
+    def prompt(self, message: str, name: Optional[str] = None) -> None:
         """
         Prompt the bot with the given user message.
 
         Args:
-            user_message (str): The message content from the user.
+            message (str): The message content from the user.
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
-        if self._thread_queue.is_alive():
-            self._openai_manager.interrupt()
-            self._text_to_speech.interrupt()
-
-        message_thread = threading.Thread(
-            target=self.send_message,
-            args=(
-                user_message,
-                name,
-            ),
-            daemon=True,
-        )
-        self._thread_queue.add_task(message_thread, unskippable=True)
+        # Do not send the message if it is empty.
+        if message.strip():
 
-        self._response_thread = threading.Thread(target=self.get_response, daemon=True)
-        self._thread_queue.add_task(self._response_thread)
+            # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
+            if self._thread_queue.is_alive():
+                self._openai_manager.interrupt()
+                self._text_to_speech.interrupt()
+                self._speech_to_text.interrupt()
+
+            message_thread = threading.Thread(
+                target=self.send_message,
+                args=(
+                    message,
+                    "user",
+                    name,
+                ),
+                daemon=True,
+            )
+            self._thread_queue.add_task(message_thread, unskippable=True)
+            self._thread_queue.add_task(threading.Thread(target=self.get_response, daemon=True))
 
-    def toggle_listen(self, name: Optional[str] = None) -> None:
+    def listener_toggle(self, name: Optional[str] = None) -> None:
         """
         Toggle the listening state of the bot. If the bot is currently listening, it will stop listening for user input
         using speech-to-text. If the bot is not currently listening, it will start listening for user input using
         speech-to-text.
 
         Args:
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
-        if self._listening:
-            self._speech_to_text.interrupt()
+        if self._listening_toggle:
+            self.listener_deactivate()
         else:
-            self._listen_thread = threading.Thread(target=self._listen, args=(name,), daemon=True)
-            self._listen_thread.start()
+            self.listener_activate(name=name)
 
-        self._listening = not self._listening
-
-    def _listen(self, name: Optional[str] = None) -> None:
+    def listener_activate(self, name: Optional[str] = None) -> None:
         """
-        Listen for user input using speech-to-text and prompt the bot with the transcribed message.
+        Activate the speech-to-text listener.
 
         Args:
             name (Optional[str]): The name of the user sending the message. Defaults to None.
         """
-        # Listen for user input using speech-to-text
-        for sentence in self._speech_to_text.listen():
-
-            # Do not send the message if it is empty.
-            if sentence.strip():
-
-                if self._thread_queue.is_alive():
-                    self._openai_manager.interrupt()
-                    self._text_to_speech.interrupt()
-
-                # Send the transcribed message to the bot
-                message_thread = threading.Thread(
-                    target=self.send_message,
-                    args=(
-                        sentence,
-                        name,
-                    ),
-                    daemon=True,
-                )
-                self._thread_queue.add_task(message_thread, unskippable=True)
-
-                self._response_thread = threading.Thread(target=self.get_response, daemon=True)
-                self._thread_queue.add_task(self._response_thread)
+        if not self._listening_toggle:
+            self._listening_toggle = True
+            self._listen_thread = threading.Thread(target=self._listen, args=(name,), daemon=True)
+            self._listen_thread.start()
 
-    def _append_to_chat_log(self, word: str) -> None:
+    def listener_deactivate(self) -> None:
         """
-        Updates the chat log with the latest output.
-
-        Args:
-            word (str): The word to be added to the conversation area.
+        Deactivate the speech-to-text listener.
         """
-        with self._log_lock:
-            with open(self._log_path, "a+") as fs:
-                fs.write(word)
+        if self._listening_toggle:
+            self._listening_toggle = False
+            self._speech_to_text.interrupt()
 
     def get_response(self) -> None:
         """
         Get a response from the bot and update the conversation area with the response. This method handles generating
         the bot's response using the OpenAIManager and updating the conversation area with the response text using
         text-to-speech synthesis.
         """
@@ -200,12 +196,80 @@
         """
         End the bot's response and update the conversation area accordingly. This method should be called after the
         bot's response has been fully generated and added to the conversation area.
         """
         self.update_conversation_area("\n\n")
 
     @abstractmethod
+    def _init_gui(self) -> None:
+        """
+        Initialize the graphical user interface for the frontend.
+        This method should be implemented by subclasses to create the specific GUI components.
+        """
+
+    @abstractmethod
+    def update_conversation_area(self, word: str) -> None:
+        """
+        Update the conversation area with the given word, and add the word to the chat log.
+        This method should be implemented by subclasses to handle updating the specific GUI components.
+
+        Args:
+            word (str): The word to add to the conversation area.
+        """
+        self._append_to_chat_log(word)
+
+    @abstractmethod
     def run(self) -> None:
         """
         Run the frontend application.
         This method should be implemented by subclasses to handle the main event loop of the specific GUI framework.
         """
+
+    def _listen(self, name: Optional[str] = None) -> None:
+        """
+        Listen for user input using speech-to-text and prompt the bot with the transcribed message.
+
+        Args:
+            name (Optional[str]): The name of the user sending the message. Defaults to None.
+        """
+        # Interrupt any currently active ChatCompletion, text-to-speech, or speech-to-text streams
+        self._speech_to_text.interrupt()
+        self._text_to_speech.interrupt()
+        self._openai_manager.interrupt()
+
+        # Flag is set to True if a new user input is detected.
+        input_detected = False
+
+        # Listen for user input using speech-to-text
+        for sentence in self._speech_to_text.listen():
+
+            # Do not send the message if it is empty.
+            if sentence.strip():
+
+                # Set the flag to True since a new user input was detected.
+                input_detected = True
+
+                # Send the transcribed message to the bot
+                message_thread = threading.Thread(
+                    target=self.send_message,
+                    args=(
+                        sentence.strip(),
+                        "user",
+                        name,
+                    ),
+                    daemon=True,
+                )
+                self._thread_queue.add_task(message_thread, unskippable=True)
+
+        if input_detected:
+            self._thread_queue.add_task(threading.Thread(target=self.get_response, daemon=True))
+
+    def _append_to_chat_log(self, word: str) -> None:
+        """
+        Updates the chat log with the latest output.
+
+        Args:
+            word (str): The word to be added to the conversation area.
+        """
+        with self._log_lock:
+            with open(self._log_path, "a+") as fs:
+                fs.write(word)
```

### Comparing `BanterBot-0.0.3/banterbot/gui/banter_bot_tk.py` & `BanterBot-0.0.4/banterbot/gui/tk_simple_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,128 @@
 import tkinter as tk
 from tkinter import ttk
+from typing import Optional
 
 from banterbot.data.azure_neural_voices import AzureNeuralVoice, get_voice_by_name
 from banterbot.data.openai_models import OpenAIModel, get_model_by_name
-from banterbot.gui.banter_bot_interface import BanterBotInterface
+from banterbot.gui.interface import Interface
 
 
-class BanterBotTK(tk.Tk, BanterBotInterface):
+class TKSimpleInterface(tk.Tk, Interface):
     """
-    BanterBotTK is a graphical user interface (GUI) for a chatbot application that uses OpenAI models for generating
+    TKSimpleInterface is a graphical user interface (GUI) for the BanterBot package that uses OpenAI models for generating
     responses, Azure Neural Voices for text-to-speech, and Azure speech-to-text recognition. The class inherits from
-    both tkinter.Tk and BanterBotInterface, providing a seamless integration of the chatbot functionality with a
-    user-friendly interface.
+    both tkinter.Tk and Interface, providing a seamless integration of the chatbot functionality with a user-friendly
+    interface.
 
     The GUI allows users to interact with the chatbot by entering their name and message, and it displays the
     conversation history in a scrollable text area. Users can send messages by pressing the "Send" button or the "Enter"
     key. The chatbot's responses are generated using the specified OpenAI model and can be played back using the
     specified Azure Neural Voice. Additionally, users can toggle speech-to-text input by pressing the "Listen" button.
     """
 
     def __init__(
         self,
         model: OpenAIModel = get_model_by_name("gpt-3.5-turbo"),
         voice: AzureNeuralVoice = get_voice_by_name("Aria"),
         style: str = "chat",
+        system: Optional[str] = None,
     ) -> None:
         """
-        Initialize the BanterBotTK class, which inherits from both tkinter.Tk and BanterBotInterface.
+        Initialize the TKSimpleInterface class, which inherits from both tkinter.Tk and Interface.
 
         Args:
             model (OpenAIModel, optional): The OpenAI model to be used for generating responses.
             voice (AzureNeuralVoice, optional): The Azure Neural Voice to be used for text-to-speech.
             style (str, optional): The style of the conversation (e.g., "cheerful", "sad", "chat").
+            system (Optional[str]): An initialization prompt that can be used to set the scene.
         """
         tk.Tk.__init__(self)
-        BanterBotInterface.__init__(self, model=model, voice=voice, style=style)
-        self._listening = False
+        Interface.__init__(self, model=model, voice=voice, style=style, system=system)
+
+        # Bind the `_quit` method to program exit, in order to guarantee the stopping of all running threads.
+        self.protocol("WM_DELETE_WINDOW", self._quit)
+
+    def update_conversation_area(self, word: str) -> None:
+        """
+        Update the conversation area with the given word.
+
+        Args:
+            word (str): The word to be added to the conversation area.
+        """
+        super().update_conversation_area(word)
+        self.conversation_area["state"] = tk.NORMAL
+        self.conversation_area.insert(tk.END, word)
+        self.conversation_area.update_idletasks()
+        self.conversation_area["state"] = tk.DISABLED
+        self.conversation_area.see(tk.END)
+
+    def select_all_on_focus(self, event) -> None:
+        """
+        Select all text in the widget when it receives focus.
+
+        Args:
+            event: The event object containing information about the focus event.
+        """
+        widget = event.widget
+        if widget == self.name_entry:
+            self._name_entry_focused = True
+            widget.selection_range(0, tk.END)
+            widget.icursor(tk.END)
+        else:
+            self._name_entry_focused = False
+
+    def prompt(self) -> None:
+        """
+        Prompt the user for input and process the message.
+        This method retrieves the user's name and message, and then calls the superclass's prompt method.
+        """
+        user_name = self.name_entry.get().split(" ")[0].strip()
+        user_message = self.message_entry.get()
+        if not user_message:
+            return
+        else:
+            super().prompt(user_message, user_name)
+            self.message_entry.delete(0, tk.END)
+
+    def listener_toggle(self) -> None:
+        """
+        Toggle the speech-to-text functionality.
+        """
+        if self._listening_toggle:
+            self.listen_btn["text"] = "Listen"
+        else:
+            self.listen_btn["text"] = "Stop"
+
+        user_name = self.name_entry.get().split(" ")[0].strip()
+        super().listener_toggle(user_name)
+
+    def run(self) -> None:
+        """
+        Run the BanterBot application.
+        This method starts the main event loop of the tkinter application.
+        """
+        self.mainloop()
+
+    def _quit(self) -> None:
+        """
+        This method is called on exit, and interrupts any currently running activity.
+        """
+        self._openai_manager.interrupt()
+        self._text_to_speech.interrupt()
+        self._speech_to_text.interrupt()
+        self.quit()
+        self.destroy()
 
     def _init_gui(self) -> None:
         """
         Initialize the graphical user interface for the BanterBot application.
         This method sets up the main window, conversation area, input fields, and buttons.
         """
-        self.title("BanterBot")
+        self.title(f"BanterBot {self._model.name}")
         self.configure(bg="black")
         self.geometry("1024x768")
         self._font = ("Cascadia Code", 16)
 
         self.style = ttk.Style()
         self.style.theme_use("clam")
         self.style.configure(".", font=self._font, bg="black", fg="white")
@@ -85,78 +161,11 @@
         self.message_entry.grid(row=0, column=1, padx=(5, 5), pady=5, sticky="nsew")
         self.message_entry.focus_set()
         self.entry_frame.columnconfigure(1, weight=1)
 
         self.send_btn = ttk.Button(self.entry_frame, text="Send", command=self.prompt, width=7)
         self.send_btn.grid(row=0, column=2, padx=(0, 5), pady=5, sticky="nsew")
 
-        self.listen_btn = ttk.Button(self.entry_frame, text="Listen", command=self.toggle_listen, width=7)
+        self.listen_btn = ttk.Button(self.entry_frame, text="Listen", command=self.listener_toggle, width=7)
         self.listen_btn.grid(row=0, column=3, padx=(0, 5), pady=5, sticky="nsew")
 
         self.message_entry.bind("<Return>", lambda event: self.prompt())
-
-    def update_conversation_area(self, word: str) -> None:
-        """
-        Update the conversation area with the given word.
-
-        Args:
-            word (str): The word to be added to the conversation area.
-        """
-        super().update_conversation_area(word)
-        self.conversation_area["state"] = tk.NORMAL
-        self.conversation_area.insert(tk.END, word)
-        self.conversation_area.update_idletasks()
-        self.conversation_area["state"] = tk.DISABLED
-        self.conversation_area.see(tk.END)
-
-    def select_all_on_focus(self, event) -> None:
-        """
-        Select all text in the widget when it receives focus.
-
-        Args:
-            event: The event object containing information about the focus event.
-        """
-        widget = event.widget
-        if widget == self.name_entry:
-            self._name_entry_focused = True
-            widget.selection_range(0, tk.END)
-            widget.icursor(tk.END)
-        else:
-            self._name_entry_focused = False
-
-    def reset_on_send(self) -> None:
-        """
-        Reset the focus state of the name entry field after sending a message.
-        """
-        self._name_entry_focused = False
-
-    def toggle_listen(self) -> None:
-        """
-        Toggle the speech-to-text functionality.
-        """
-        if self.listening:
-            self.listen_btn["text"] = "Listen"
-        else:
-            self.listen_btn["text"] = "Stop"
-
-        user_name = self.name_entry.get().split(" ")[0].strip()
-        super().toggle_listen(user_name)
-
-    def prompt(self) -> None:
-        """
-        Prompt the user for input and process the message.
-        This method retrieves the user's name and message, and then calls the superclass's prompt method.
-        """
-        user_name = self.name_entry.get().split(" ")[0].strip()
-        user_message = self.message_entry.get()
-        if not user_message:
-            return
-        else:
-            super().prompt(user_message, user_name)
-            self.message_entry.delete(0, tk.END)
-
-    def run(self) -> None:
-        """
-        Run the BanterBot application.
-        This method starts the main event loop of the tkinter application.
-        """
-        self.mainloop()
```

### Comparing `BanterBot-0.0.3/banterbot/gui/cli.py` & `BanterBot-0.0.4/banterbot/gui/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 
 from banterbot.data.openai_models import get_model_by_name
-from banterbot.gui.banter_bot_tk import BanterBotTK
+from banterbot.gui.tk_multiplayer_interface import TKMultiplayerInterface
+from banterbot.gui.tk_simple_interface import TKSimpleInterface
 
 
 def run() -> None:
     """
     The main function to run the BanterBot Command Line Interface.
 
     This function parses command line arguments, sets up the necessary configurations, and initializes the BanterBotTK
@@ -26,22 +27,44 @@
             "2) AZURE_SPEECH_KEY: A valid Azure Cognitive Services Speech API key for text-to-speech and "
             "speech-to-text functionality,\n"
             "3) AZURE_SPEECH_REGION: The region associated with your Azure Cognitive Services Speech API key."
         ),
     )
 
     parser.add_argument(
+        "-s",
+        "--system",
+        action="store",
+        type=str,
+        dest="system",
+        help="Adds a system message to the beginning of the conversation; can help to set the scene.",
+    )
+
+    parser.add_argument(
         "-g",
         "--gpt4",
         action="store_true",
         dest="gpt4",
         help="Enable GPT-4; only works if you have GPT-4 API access.",
     )
 
-    args=parser.parse_args()
+    parser.add_argument(
+        "-m",
+        "--multiplayer",
+        action="store_true",
+        dest="mp",
+        help="Enables the pre-release multiplayer interface; multiplayer is not fully implemented and may be buggy.",
+    )
+
+    args = parser.parse_args()
 
     kwargs = {
         "model": get_model_by_name("gpt-4") if args.gpt4 else get_model_by_name("gpt-3.5-turbo"),
+        "system": args.system,
     }
 
-    gui = BanterBotTK(**kwargs)
-    gui.run()
+    if args.mp:
+        interface = TKMultiplayerInterface(**kwargs)
+    else:
+        interface = TKSimpleInterface(**kwargs)
+
+    interface.run()
```

### Comparing `BanterBot-0.0.3/banterbot/utils/message.py` & `BanterBot-0.0.4/banterbot/utils/message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.3/banterbot/utils/nlp.py` & `BanterBot-0.0.4/banterbot/utils/nlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Tuple
 
 import spacy
-
 from banterbot.data.enums import SpaCyLangModel
 
 
 class NLP:
     """
     A comprehensive toolkit that provides a set of Natural Language Processing utilities. It leverages the capabilities
     of the SpaCy package. The toolkit is designed to automatically download the necessary models if they are not
```

### Comparing `BanterBot-0.0.3/banterbot/utils/speech_to_text_output.py` & `BanterBot-0.0.4/banterbot/utils/speech_to_text_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import json
 from typing import Iterator, List, TypedDict
 
 import azure.cognitiveservices.speech as speechsdk
-
 from banterbot.data.azure_neural_voices import AzureNeuralVoice
 from banterbot.data.enums import SpeechProcessingType, WordCategory
 from banterbot.utils.nlp import NLP
 from banterbot.utils.word import Word
 
 
 class WordJSON(TypedDict):
```

### Comparing `BanterBot-0.0.3/banterbot/utils/text_to_speech_output.py` & `BanterBot-0.0.4/banterbot/utils/text_to_speech_output.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.3/banterbot/utils/thread_queue.py` & `BanterBot-0.0.4/banterbot/utils/thread_queue.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,36 +11,14 @@
     new task is added unless it is declared unskippable.
     """
 
     def __init__(self):
         self._lock = threading.Lock()
         self._event_queue: List[threading.Event] = []
 
-    def _thread_wrapper(self, thread: threading.Thread, index: int, unskippable: bool) -> None:
-        """
-        A wrapper function for executing threads in the queue.
-
-        This function is responsible for waiting for the previous task to complete before starting the current task, and
-        setting the event for the next task in the queue. If the current task is skippable and not the last task in the
-        queue, it will not be executed.
-
-        Args:
-            thread (threading.Thread): The thread to be executed.
-            index (int): The index of the thread in the event queue.
-            unskippable (bool): Whether the thread should be executed even if a new task is added to the queue.
-        """
-        if index > 0:
-            self._event_queue[index - 1].wait()
-
-        if unskippable or index == len(self._event_queue) - 1:
-            thread.start()
-            thread.join()
-
-        self._event_queue[index].set()
-
     def is_alive(self) -> bool:
         """
         Check if the last task in the queue is still running.
 
         Returns:
             bool: True if the last task is still running, False otherwise.
         """
@@ -65,7 +43,29 @@
             index = len(self._event_queue)
             self._event_queue.append(threading.Event())
 
         wrapper_thread = threading.Thread(
             target=self._thread_wrapper, args=(thread, index, unskippable), daemon=thread.daemon
         )
         wrapper_thread.start()
+
+    def _thread_wrapper(self, thread: threading.Thread, index: int, unskippable: bool) -> None:
+        """
+        A wrapper function for executing threads in the queue.
+
+        This function is responsible for waiting for the previous task to complete before starting the current task, and
+        setting the event for the next task in the queue. If the current task is skippable and not the last task in the
+        queue, it will not be executed.
+
+        Args:
+            thread (threading.Thread): The thread to be executed.
+            index (int): The index of the thread in the event queue.
+            unskippable (bool): Whether the thread should be executed even if a new task is added to the queue.
+        """
+        if index > 0:
+            self._event_queue[index - 1].wait()
+
+        if unskippable or index == len(self._event_queue) - 1:
+            thread.start()
+            thread.join()
+
+        self._event_queue[index].set()
```

### Comparing `BanterBot-0.0.3/banterbot/utils/word.py` & `BanterBot-0.0.4/banterbot/utils/word.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 from dataclasses import dataclass
 from typing import Optional
 
 import azure.cognitiveservices.speech as speechsdk
-
 from banterbot.data.enums import SpeechProcessingType, WordCategory
 
 
 @dataclass(frozen=True)
 class Word:
     """
     This class encapsulates a word in the output of a text-to-speech synthesis or input from a speech-to-text
```

### Comparing `BanterBot-0.0.3/setup.py` & `BanterBot-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 def run_tests():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover("tests", pattern="test_*.py")
     return test_suite
 
-version = "0.0.3"
+
+version = "0.0.4"
 setup(
     name="BanterBot",
     packages=find_packages(),
     test_suite="setup.run_tests",
     version=version,
     description=description,
     long_description=long_description,
```

### Comparing `BanterBot-0.0.3/tests/core/test_openai_manager.py` & `BanterBot-0.0.4/tests/core/test_openai_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 import os
 import unittest
 from dataclasses import dataclass
 from unittest.mock import patch
 
 import openai
-
 from banterbot.core.openai_manager import OpenAIManager
 from banterbot.data.openai_models import OpenAIModel
 from banterbot.utils.message import Message
 from banterbot.utils.nlp import NLP
 
 
 @dataclass
```

### Comparing `BanterBot-0.0.3/tests/core/test_text_to_speech.py` & `BanterBot-0.0.4/tests/core/test_text_to_speech.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 from unittest.mock import MagicMock, patch
 
 from azure.cognitiveservices.speech import SpeechSynthesisBoundaryType, SpeechSynthesisOutputFormat, SpeechSynthesizer
-
 from banterbot.core.text_to_speech import TextToSpeech
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 
 
 class TestTextToSpeech(unittest.TestCase):
     def setUp(self):
         self.tts = TextToSpeech()
```

### Comparing `BanterBot-0.0.3/tests/utils/test_message.py` & `BanterBot-0.0.4/tests/utils/test_message.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.3/tests/utils/test_nlp.py` & `BanterBot-0.0.4/tests/utils/test_nlp.py`

 * *Files identical despite different names*

### Comparing `BanterBot-0.0.3/tests/utils/test_text_to_speech_output.py` & `BanterBot-0.0.4/tests/utils/test_text_to_speech_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 appending new words, stopping the output process, and streaming words from the output.
 """
 import datetime
 import unittest
 from typing import List
 
 import azure.cognitiveservices.speech as speechsdk
-
 from banterbot.utils.text_to_speech_output import TextToSpeechOutput
 from banterbot.utils.text_to_speech_word import TextToSpeechWord
 
 
 class TextToSpeechOutputTestCase(unittest.TestCase):
     def setUp(self):
         self.output = TextToSpeechOutput("Hello, world!")
```

### Comparing `BanterBot-0.0.3/tests/utils/test_text_to_speech_word.py` & `BanterBot-0.0.4/tests/utils/test_text_to_speech_word.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 as a string representation.
 """
 import datetime
 import unittest
 from dataclasses import dataclass
 
 import azure.cognitiveservices.speech as speechsdk
-
 from banterbot.utils.text_to_speech_word import TextToSpeechWord
 
 
 @dataclass(frozen=True)
 class MockSpeechSynthesisBoundaryType:
     WORD = "word"
     PUNCTUATION = "punctuation"
```

### Comparing `BanterBot-0.0.3/tests/utils/test_thread_queue.py` & `BanterBot-0.0.4/tests/utils/test_thread_queue.py`

 * *Files identical despite different names*

