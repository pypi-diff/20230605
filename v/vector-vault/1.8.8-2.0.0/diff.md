# Comparing `tmp/vector_vault-1.8.8.tar.gz` & `tmp/vector_vault-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.8.tar", last modified: Mon Jun  5 02:11:12 2023, max compression
+gzip compressed data, was "vector_vault-2.0.0.tar", last modified: Mon Jun  5 09:16:26 2023, max compression
```

## Comparing `vector_vault-1.8.8.tar` & `vector_vault-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.628578 vector_vault-1.8.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-05 02:11:12.628430 vector_vault-1.8.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-05 02:11:12.628620 vector_vault-1.8.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-05 02:10:45.000000 vector_vault-1.8.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.626680 vector_vault-1.8.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-05 02:11:12.000000 vector_vault-1.8.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 02:11:12.628230 vector_vault-1.8.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    13363 2023-06-05 02:09:13.000000 vector_vault-1.8.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-05 02:10:12.000000 vector_vault-1.8.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-05 02:10:06.000000 vector_vault-1.8.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.8/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    27815 2023-06-05 02:10:21.000000 vector_vault-1.8.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-1.8.8/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.076345 vector_vault-2.0.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-2.0.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-05 09:16:26.076166 vector_vault-2.0.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19513 2023-06-05 09:15:29.000000 vector_vault-2.0.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-05 09:16:26.076385 vector_vault-2.0.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-05 09:16:17.000000 vector_vault-2.0.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.073530 vector_vault-2.0.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20238 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-05 09:16:26.000000 vector_vault-2.0.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-05 09:16:26.075892 vector_vault-2.0.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-2.0.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    13363 2023-06-05 02:09:13.000000 vector_vault-2.0.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-05 02:10:12.000000 vector_vault-2.0.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-2.0.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-2.0.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1782 2023-06-05 02:10:06.000000 vector_vault-2.0.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-2.0.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    27814 2023-06-05 02:29:22.000000 vector_vault-2.0.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3938 2023-06-04 22:35:53.000000 vector_vault-2.0.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-2.0.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.8/LICENSE` & `vector_vault-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/PKG-INFO` & `vector_vault-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: vector_vault
-Version: 1.8.8
-Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
-Home-page: https://github.com/John-Rood/VectorVault
-Author: VectorVault.io
-Author-email: john@johnrood.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
 By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
@@ -37,15 +18,15 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We process vectors in the cloud
 <br>
 `get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
@@ -129,15 +110,16 @@
 <br>
 
 # Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-Since your vault lives in the cloud, making a call to it is really easy. You can even do it by command line:
+You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
+Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
 curl -X POST "https://api.vectorvault.io/get_similar" \
      -H "Content-Type: application/json" \
      -d '{
         "user": "your_username",
         "api_key": "your_api_key",
         "vault": "your_vault_name",
@@ -254,151 +236,89 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
-<br>
-
-# Metadata Made Easy
-
-Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
-```
-meta = {
-    'name': 'Lifestyle in LA',
-    'country': 'United State',
-    'city': 'LA' 
-}
-
-vault.add(text, meta)
-
-vault.get_vectors()
-
-vault.save()
-```
 
+# Streaming:
+Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
-```
-vault.add(text, name='Lifestyle in LA')
-
-vault.get_vectors()
+![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
 
-vault.save()
-```
+## get_chat_stream():
 
-<br>
+Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
+Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
+`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
+`print_stream()` is for local console printing.
 
-To find the name later:
-```
-similar_data = vault.get_similar("Your text input") 
+Example Signle Usage: 
+`response = vault.print_stream(vault.get_chat_stream(text))`
 
-for result in similar_data:
-    print(result['metadata']['name'])
-```
->> Lifestyle in LA Lifestyle in LA Lifestyle in LA Lifestyle in LA
-<br>
-
-### Add Any Meta Fields & Retrieve later
-Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Create a dictionary containing all the information about the book. Save all that to the vault. Now when calling `get_similar()` or `get_chat(text, get_context=True, return_context=True)` the vault will return texts from the book and the metadata will have what you need to know. 
+Example Chat: 
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
+Example Summary: 
+`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
 
-```
-with open('1984.txt', 'r') as file:
-    text = file.read()
+Example Context-Based Response:
+`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
 
-book_metadata = {
-    'title': '1984',
-    'author': 'George Orwell',
-    'genre': 'Dystopian',
-    'publication_year': 1949,
-    'publisher': 'Secker & Warburg',
-    'ISBN': '978-0451524935',
-    'language': 'English',
-    'page_count': 328
-}
+Example Context-Based Response w/ Chat History:
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
 
-vault.add(text, book_metadata)
+Example Context-Response with Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
 
-vault.get_vectors()
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
-vault.save()
-```
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
-<br>
+Response is a always a stream
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
 
-To find the metadata later:
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
+## get_chat()
+print(vault.get_chat(text, history)
 
-for result in similar_data:
-    print(result['metadata']['title'])
-    print(result['metadata']['author'])
-    print(result['metadata']['genre'])
+## get_chat_stream()
+for word in vault.get_chat_stream(text, history):
+        print(word)
 ```
->> 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian
-
-^ list is always returned, so you can do like above or like below...
-
+This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
-print(similar_data[0]['metadata']['title'])
+vault.print_stream(vault.get_chat_stream(text, history))
 ```
->> 1984
-
-<br>
 <br>
 
-# Change Vaults
-
-In this example science vault, we will print a list of vaults in the current vault directory
-```
-science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
-
-print(science_vault.get_vaults())
-```
->> ['biology', 'physics', 'chemistry']
-
-
-## Access vaults within vaults
-
-- biology vault within science vault
-```
-biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
-```
-
-- chemistry vault within science vault
-```
-chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
-
-print(chemistry_vault.get_vaults())
-```
->> ['reactions', 'formulas', 'lab notes']
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
 
 
-- lab notes vault within chemistry vault
-```
-lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
-```
+<br>
+<br> 
 
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -419,14 +339,15 @@
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
+<br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
@@ -439,36 +360,34 @@
 ## Getting Started:
 Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+### If have any questions, drop a message in the Vector Vault [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 Happy coding!
 <br>
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
 <br>
 
 
 ## FAQ
 <br>
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
+37 full length book texts with vectors make up ~250MB of storage with around 10,000 - 15,000 items of 1000+ characters for each item. This example of 37 books is considered small. Personal plans come with 1GB of storage, so this doesn't even come close to plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. Running locally, you can expect ~0.7 seconds. Just referencing the cloud, you can expect ~1 second. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small. You can try our app at the bottom of our [website](https://vectorvault.io) to see the latency for yourself. Keep in mind that if you do so, you will be seeing the latency from chatgpt on top of the vault time, but it's still so fast that its not noticible during a conversation. If you had 10 times that much data, api latency may be around 2 seconds max, so still fast enough for realtime conversations. Or you can just get an Enterprise Cloud Plan from us and get it even faster.
 
 <br>
 
 ### How should I segment my data?
-Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets.
 
 <br>
 
 ### What if I'm a large company with very large data
-If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
-
-
+If you need to store more than 1 gig of data in single vaults for any reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need. It is always active and scalable to terabytes. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up ~8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
```

### Comparing `vector_vault-1.8.8/README.md` & `vector_vault-2.0.0/vector_vault.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: vector-vault
+Version: 2.0.0
+Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
+Home-page: https://github.com/John-Rood/VectorVault
+Author: VectorVault.io
+Author-email: john@johnrood.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![alt text](https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/297fde6c-f5b4-4076-83bc-81dcfdbffebe/Vector+Vault+Header+5000.jpg)
 
 Vector Vault is a cloud vector database service that was built to make generative ai chat quick and easy. It allows users to vectorize data easily and access them seamlessly from the cloud. It's suitable for both small projects and large. Vector Vault has been designed with a user-friendly code interface to make the process of working with vector data easy and let you focus on what matters, results. Vector Vault ensures secure and isolated data handling and enables you to create and interact vector databases - aka "vaults" - in the cloud, at millisecond response times.
 
 By combining vector similarity search with generative ai chat, new possibilities for conversation and communication emerge. For example, product information can be added to a vault, and when a customer asks a product question, the right product information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This capability allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news, to ai code reviews that reference source documentation, to ai domain experts for specific knowledge sets, and much more.
 
 Vector Vault uses a proprietary architecture, called "Inception", allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault api key in order to access the cloud vaults. If you don't already have one, you can use the included `register()` function or sign up at [VectorVault.io](https://vectorvault.io)
@@ -18,15 +37,15 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We process vectors in the cloud
 <br>
 `get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
@@ -110,15 +129,16 @@
 <br>
 
 # Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-Since your vault lives in the cloud, making a call to it is really easy. You can even do it by command line:
+You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
+Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
 curl -X POST "https://api.vectorvault.io/get_similar" \
      -H "Content-Type: application/json" \
      -d '{
         "user": "your_username",
         "api_key": "your_api_key",
         "vault": "your_vault_name",
@@ -235,151 +255,89 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
-<br>
-
-# Metadata Made Easy
-
-Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
-```
-meta = {
-    'name': 'Lifestyle in LA',
-    'country': 'United State',
-    'city': 'LA' 
-}
-
-vault.add(text, meta)
-
-vault.get_vectors()
-
-vault.save()
-```
 
+# Streaming:
+Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
-```
-vault.add(text, name='Lifestyle in LA')
-
-vault.get_vectors()
+![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
 
-vault.save()
-```
+## get_chat_stream():
 
-<br>
+Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
+Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
+`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
+`print_stream()` is for local console printing.
 
-To find the name later:
-```
-similar_data = vault.get_similar("Your text input") 
+Example Signle Usage: 
+`response = vault.print_stream(vault.get_chat_stream(text))`
 
-for result in similar_data:
-    print(result['metadata']['name'])
-```
->> Lifestyle in LA Lifestyle in LA Lifestyle in LA Lifestyle in LA
-<br>
-
-### Add Any Meta Fields & Retrieve later
-Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Create a dictionary containing all the information about the book. Save all that to the vault. Now when calling `get_similar()` or `get_chat(text, get_context=True, return_context=True)` the vault will return texts from the book and the metadata will have what you need to know. 
+Example Chat: 
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
+Example Summary: 
+`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
 
-```
-with open('1984.txt', 'r') as file:
-    text = file.read()
+Example Context-Based Response:
+`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
 
-book_metadata = {
-    'title': '1984',
-    'author': 'George Orwell',
-    'genre': 'Dystopian',
-    'publication_year': 1949,
-    'publisher': 'Secker & Warburg',
-    'ISBN': '978-0451524935',
-    'language': 'English',
-    'page_count': 328
-}
+Example Context-Based Response w/ Chat History:
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
 
-vault.add(text, book_metadata)
+Example Context-Response with Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
 
-vault.get_vectors()
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
-vault.save()
-```
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
-<br>
+Response is a always a stream
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
 
-To find the metadata later:
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
+## get_chat()
+print(vault.get_chat(text, history)
 
-for result in similar_data:
-    print(result['metadata']['title'])
-    print(result['metadata']['author'])
-    print(result['metadata']['genre'])
+## get_chat_stream()
+for word in vault.get_chat_stream(text, history):
+        print(word)
 ```
->> 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian
-
-^ list is always returned, so you can do like above or like below...
-
+This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
-print(similar_data[0]['metadata']['title'])
+vault.print_stream(vault.get_chat_stream(text, history))
 ```
->> 1984
-
-<br>
 <br>
 
-# Change Vaults
-
-In this example science vault, we will print a list of vaults in the current vault directory
-```
-science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
-
-print(science_vault.get_vaults())
-```
->> ['biology', 'physics', 'chemistry']
-
-
-## Access vaults within vaults
-
-- biology vault within science vault
-```
-biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
-```
-
-- chemistry vault within science vault
-```
-chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
-
-print(chemistry_vault.get_vaults())
-```
->> ['reactions', 'formulas', 'lab notes']
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
 
 
-- lab notes vault within chemistry vault
-```
-lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
-```
+<br>
+<br> 
 
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -400,14 +358,15 @@
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
+<br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
@@ -420,34 +379,36 @@
 ## Getting Started:
 Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+### If have any questions, drop a message in the Vector Vault [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 Happy coding!
 <br>
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
 <br>
 
 
 ## FAQ
 <br>
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
+37 full length book texts with vectors make up ~250MB of storage with around 10,000 - 15,000 items of 1000+ characters for each item. This example of 37 books is considered small. Personal plans come with 1GB of storage, so this doesn't even come close to plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. Running locally, you can expect ~0.7 seconds. Just referencing the cloud, you can expect ~1 second. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small. You can try our app at the bottom of our [website](https://vectorvault.io) to see the latency for yourself. Keep in mind that if you do so, you will be seeing the latency from chatgpt on top of the vault time, but it's still so fast that its not noticible during a conversation. If you had 10 times that much data, api latency may be around 2 seconds max, so still fast enough for realtime conversations. Or you can just get an Enterprise Cloud Plan from us and get it even faster.
 
 <br>
 
 ### How should I segment my data?
-Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets.
 
 <br>
 
 ### What if I'm a large company with very large data
-If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+If you need to store more than 1 gig of data in single vaults for any reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need. It is always active and scalable to terabytes. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up ~8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+
+
```

### Comparing `vector_vault-1.8.8/setup.py` & `vector_vault-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.8",
+    version="2.0.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vector-vault
-Version: 1.8.8
+Name: vector_vault
+Version: 2.0.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -37,15 +37,15 @@
 <br>
 `save()` : Saves the data with embeddings to the Vault (cloud), along with any metadata
 <br>
 `delete()` : Deletes the current Vault and all contents
 <br>
 `get_vaults()` : Retrieves a list of Vaults within the current Vault directory
 <br>
-`get_similar()` : Retrieves similar texts from the Vault for a given input text - We processes vectors in the cloud
+`get_similar()` : Retrieves similar texts from the Vault for a given input text - We process vectors in the cloud
 <br>
 `get_similar_local()` : Retrieves similar texts from the Vault for a given input text - You process vectors locally
 <br>
 `get_chat()` : Retrieves a response from ChatGPT, with support for handling conversation history, summarizing responses, and retrieving context-based responses by referencing similar data in the vault
 
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
@@ -129,15 +129,16 @@
 <br>
 
 # Call Your Vault:
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/5ae905b0-43d0-4b86-a965-5b447ee8c7de/Vector+Vault+Vault.jpg?content-type=image%2Fjpeg" width="60%" height="60%" />
 </p>
 
-Since your vault lives in the cloud, making a call to it is really easy. You can even do it by command line:
+You can create a javascript or HTML post to `"https://api.vectorvault.io/get_similar"`, to run front end apps.
+Since your Vault lives in the cloud, making a call to it is really easy. You can even do it with a `curl` from command line:
 ```
 curl -X POST "https://api.vectorvault.io/get_similar" \
      -H "Content-Type: application/json" \
      -d '{
         "user": "your_username",
         "api_key": "your_api_key",
         "vault": "your_vault_name",
@@ -254,151 +255,89 @@
     summary = vault.get_chat(summary, summary=True)
 ```
 ^ in the above example, we make a summary, then we enter while loop that continues until the summary recieved back is a certain lenght. You could use this to summarize a 1000 page book to less than 1000 characters of text. 
 
 <br>
 <br>
 <br>
-<br>
-
-# Metadata Made Easy
-
-Metadata is useful later, when you make a call to the vault and want to know specifics about the data you got back. To add metadata to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so the name field in the metadata always exists)
-```
-meta = {
-    'name': 'Lifestyle in LA',
-    'country': 'United State',
-    'city': 'LA' 
-}
-
-vault.add(text, meta)
-
-vault.get_vectors()
-
-vault.save()
-```
 
+# Streaming:
+Use the built-in streaming functionality to get interactive chat streaming. Here's an [app](https://philbrosophy.web.app) we built to showcase what you can do with Vector Vault:
 <br>
 
-To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
-```
-vault.add(text, name='Lifestyle in LA')
+![Alt text](https://github.com/John-Rood/VectorVault/blob/main/examples/Streaming%20Demo%20Offish.gif)
 
-vault.get_vectors()
+## get_chat_stream():
 
-vault.save()
-```
+Example Usage: `vault.print_stream(vault.get_chat_stream(text))`
+Always use this `get_chat_stream()` wrapped by either `print_stream()` or `cloud_stream()`.
+`cloud_stream()` is for cloud functions, like a flask app serving a front end elsewhere.
+`print_stream()` is for local console printing.
 
-<br>
+Example Signle Usage: 
+`response = vault.print_stream(vault.get_chat_stream(text))`
 
-To find the name later:
-```
-similar_data = vault.get_similar("Your text input") 
+Example Chat: 
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history))`
 
-for result in similar_data:
-    print(result['metadata']['name'])
-```
->> Lifestyle in LA Lifestyle in LA Lifestyle in LA Lifestyle in LA
-<br>
+Example Summary: 
+`summary = vault.print_stream(vault.get_chat_stream(text, summary=True))`
 
-### Add Any Meta Fields & Retrieve later
-Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Create a dictionary containing all the information about the book. Save all that to the vault. Now when calling `get_similar()` or `get_chat(text, get_context=True, return_context=True)` the vault will return texts from the book and the metadata will have what you need to know. 
+Example Context-Based Response:
+`response = vault.print_stream(vault.get_chat_stream(text, get_context = True))`
 
+Example Context-Based Response w/ Chat History:
+`response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True))`
 
-```
-with open('1984.txt', 'r') as file:
-    text = file.read()
+Example Context-Response with Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True))`
 
-book_metadata = {
-    'title': '1984',
-    'author': 'George Orwell',
-    'genre': 'Dystopian',
-    'publication_year': 1949,
-    'publisher': 'Secker & Warburg',
-    'ISBN': '978-0451524935',
-    'language': 'English',
-    'page_count': 328
-}
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
 
-vault.add(text, book_metadata)
+Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
+`vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
 
-vault.get_vectors()
+Response is a always a stream
+`vault.get_chat_stream` will start a chat stream. The input parameters are mostly like the regular get_chat functionality, and the capabilites are all the same. The only difference is that the get_chat function returns the whole reply message at once. The get_chat_stream `yield`s each word as it it received. This means that using `get_chat_stream()` is very different than using `get_chat()`. Here's an example that prints the same message:
 
-vault.save()
 ```
+## get_chat()
+print(vault.get_chat(text, history)
 
-<br>
-
-To find the metadata later:
+## get_chat_stream()
+for word in vault.get_chat_stream(text, history):
+        print(word)
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
-
-for result in similar_data:
-    print(result['metadata']['title'])
-    print(result['metadata']['author'])
-    print(result['metadata']['genre'])
-```
->> 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian 1984 George Orwell Dystopian
-
-^ list is always returned, so you can do like above or like below...
-
+This will take each word yielded and print it as it comes in. However, that will not look good, so it's best to use the built in print function `print_stream`. 
 ```
-similar_data = vault.get_similar("How will the government control you in the future?") 
-print(similar_data[0]['metadata']['title'])
+vault.print_stream(vault.get_chat_stream(text, history))
 ```
->> 1984
-
 <br>
-<br>
-
-# Change Vaults
-
-In this example science vault, we will print a list of vaults in the current vault directory
-```
-science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
-
-print(science_vault.get_vaults())
-```
->> ['biology', 'physics', 'chemistry']
 
+Because streaming is a key functionality for end user applications, we also have a `cloud_stream` function to make cloud streaming to your front end app easy. In a flask app, your return would look like: `return Response(vault.cloud_stream(vault.get_chat_stream(text, history, get_context=True)), mimetype='text/event-stream')`
+This makes going live with highly functional cloud apps really easy. Now you can build impressive applications in record time! If have any questions, message in [Discord](https://discord.gg/AkMsP9Uq).
 
-## Access vaults within vaults
 
-- biology vault within science vault
-```
-biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
-```
-
-- chemistry vault within science vault
-```
-chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
-
-print(chemistry_vault.get_vaults())
-```
->> ['reactions', 'formulas', 'lab notes']
-
-
-- lab notes vault within chemistry vault
-```
-lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
-```
+<br>
+<br> 
 
 
 
 <br>
 <br>
 <br>
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a cloud Vault. (We load the company support texts from a .txt file, vectorize them, then add them to the Vault). As new people message in, we will vector search the Vault for similar questions and answers. We take the past answers returned from the Vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -419,14 +358,15 @@
 And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
 question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
+<br>
 
 That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
@@ -439,36 +379,36 @@
 ## Getting Started:
 Open the [examples folder](https://github.com/John-Rood/VectorVault/tree/main/examples) and try out the Google Colab tutorials we have! They will show you a lot, plus they are in Google Colab, so no local set up required, just open them up and press play.
 
 <br>
 <br>
 
 ## Contact:
-### If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+### If have any questions, drop a message in the Vector Vault [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
 
 Happy coding!
 <br>
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/7d1a596b-7560-446b-aa69-1827819d198b/Looking+out+with+hope+vector+vault.png" width="60%" height="60%" />
 </p>
 
 <br>
 
 
 ## FAQ
 <br>
 
 ### What is the latency on large datasets?
-To conceptualize "large", 37 full length book texts with vectors make up ~80MB of storage with around 10,000 - 15,000 items of ~1000 characters for each item. This example of 37 books is considered small. Free plans come with 1GB of storage, and 100MB/mo of uploading, so this doesn't even hit the free plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small.  If you had 10 times that much data, api latency may be around 5 seconds. Our architechture is optimized for lightning fast responses on small-medium size datasets, so if your data size grows to large amounts, and you see the call time taking too long, its recommended that you segment you data into multiple vaults to keep latency to 1 second on api calls. 
+37 full length book texts with vectors make up ~250MB of storage with around 10,000 - 15,000 items of 1000+ characters for each item. This example of 37 books is considered small. Personal plans come with 1GB of storage, so this doesn't even come close to plan limit. Calling similar items from this vault is one second response time - with vectors retreived, vectors searched, then similar items returned. Running locally, you can expect ~0.7 seconds. Just referencing the cloud, you can expect ~1 second. This example is about the same amount of data as the entire customer support history for any given company. So if you build a typical customer service chatbot, your vault size will be considered small. You can try our app at the bottom of our [website](https://vectorvault.io) to see the latency for yourself. Keep in mind that if you do so, you will be seeing the latency from chatgpt on top of the vault time, but it's still so fast that its not noticible during a conversation. If you had 10 times that much data, api latency may be around 2 seconds max, so still fast enough for realtime conversations. Or you can just get an Enterprise Cloud Plan from us and get it even faster.
 
 <br>
 
 ### How should I segment my data?
-Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets. *Keep in mind this only applies to very large data sets.* Also, if your data set is large and you don't mind a little longer response times on vault call, then you don't need to do anything. In that case, you can just add it all to one vault and not worry about it. 
+Vaults within vaults is the optimal structure for segmenting data. If a vault grows too large, just make multiple child vaults within the current vault directory, and store the data there. If your 'Science' vault grows too large, split it into multiple child vaults, like 'Science/Chemistry', etc - this accesses a "Chemistry" vault within the Science vault. Now you can fine grain datasets, where every child vault contains more specific subject information than the parent vault. This segmenting structure allows you to focus data on large data sets.
 
 <br>
 
 ### What if I'm a large company with very large data
-If you need to store large amounts of data in single vaults for whatever reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need, that is always active. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up about 8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
+If you need to store more than 1 gig of data in single vaults for any reason, let us know and we can set you up with Enterprise Cloud Plan. In our Enterprise plan, we create a persistent storage pod with as much memory as you need. It is always active and scalable to terabytes. With an Enterprise plan, a billion vectors search will respond in one second. For reference, the full text of 3.7 million books would be ~1.1 billion vectors, and take up ~8 terabytes of storage. If this is what you're looking for, just reach out to us by email at support at vectorvault.io.
```

### Comparing `vector_vault-1.8.8/vectorvault/__init__.py` & `vector_vault-2.0.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/ai.py` & `vector_vault-2.0.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/cloudmanager.py` & `vector_vault-2.0.0/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/creds.py` & `vector_vault-2.0.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/download.py` & `vector_vault-2.0.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/itemize.py` & `vector_vault-2.0.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/signup.py` & `vector_vault-2.0.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/vault.py` & `vector_vault-2.0.0/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,14 @@
             Example Context-Response with SPECIFIC META TAGS for Context Samples Returned:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author']))`
             
             Example Context-Response with SPECIFIC META TAGS for Context Samples Returned & Specific Meta Prefixes and Suffixes:
             `vault_response = vault.print_stream(vault.get_chat_stream(text, get_context = True, return_context = True, include_context_meta=True, metatag=['title', 'author'], metatag_prefixes=['\n\n Title: ', '\nAuthor: '], metatag_suffixes=['', '\n']))`
             
             Response is a always a stream
-
         '''
 
         start_time = time.time()
         if not self.last_chat_time:
             self.last_chat_time = start_time - 20
         
         if not self.needed_sleep_time:
```

### Comparing `vector_vault-1.8.8/vectorvault/vecreq.py` & `vector_vault-2.0.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.8/vectorvault/wrap.py` & `vector_vault-2.0.0/vectorvault/wrap.py`

 * *Files identical despite different names*

