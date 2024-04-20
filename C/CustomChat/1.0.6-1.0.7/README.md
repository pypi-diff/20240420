# Comparing `tmp/CustomChat-1.0.6.tar.gz` & `tmp/CustomChat-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomChat-1.0.6.tar", last modified: Mon Apr  1 22:49:30 2024, max compression
+gzip compressed data, was "CustomChat-1.0.7.tar", last modified: Fri Apr 19 13:00:46 2024, max compression
```

## Comparing `CustomChat-1.0.6.tar` & `CustomChat-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:49:30.761866 CustomChat-1.0.6/
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:49:30.761866 CustomChat-1.0.6/CustomChat/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 17:34:56.000000 CustomChat-1.0.6/CustomChat/Name.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       80 2024-03-31 21:26:32.000000 CustomChat-1.0.6/CustomChat/__init__.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)    30999 2024-04-01 22:36:01.000000 CustomChat-1.0.6/CustomChat/app.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      189 2024-03-02 23:52:49.000000 CustomChat-1.0.6/CustomChat/configuration.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      943 2024-04-01 22:36:12.000000 CustomChat-1.0.6/CustomChat/main.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:30.000000 CustomChat-1.0.6/CustomChat/new_com.py
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-03-31 21:40:13.000000 CustomChat-1.0.6/CustomChat/new_words.py
-drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-01 22:49:30.761866 CustomChat-1.0.6/CustomChat.egg-info/
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     3018 2024-04-01 22:49:30.000000 CustomChat-1.0.6/CustomChat.egg-info/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      348 2024-04-01 22:49:30.000000 CustomChat-1.0.6/CustomChat.egg-info/SOURCES.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-01 22:49:30.000000 CustomChat-1.0.6/CustomChat.egg-info/dependency_links.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-01 22:49:30.000000 CustomChat-1.0.6/CustomChat.egg-info/requires.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-01 22:49:30.000000 CustomChat-1.0.6/CustomChat.egg-info/top_level.txt
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     1186 2024-03-09 18:39:04.000000 CustomChat-1.0.6/LICENSE
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     3018 2024-04-01 22:49:30.761866 CustomChat-1.0.6/PKG-INFO
--rw-rw-r--   0 elliot    (1000) elliot    (1000)     2492 2024-04-01 22:47:06.000000 CustomChat-1.0.6/README.md
--rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-01 22:49:30.761866 CustomChat-1.0.6/setup.cfg
--rw-rw-r--   0 elliot    (1000) elliot    (1000)      805 2024-04-01 22:48:59.000000 CustomChat-1.0.6/setup.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-19 13:00:46.655332 CustomChat-1.0.7/
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-19 13:00:46.651333 CustomChat-1.0.7/CustomChat/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       10 2024-04-05 22:31:53.000000 CustomChat-1.0.7/CustomChat/Name.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      135 2024-04-19 12:15:58.000000 CustomChat-1.0.7/CustomChat/__init__.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       55 2024-04-19 12:49:33.000000 CustomChat-1.0.7/CustomChat/ai_data.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)    31433 2024-04-19 11:59:13.000000 CustomChat-1.0.7/CustomChat/app.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      189 2024-04-19 12:15:55.000000 CustomChat-1.0.7/CustomChat/configuration.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1567 2024-04-19 12:14:50.000000 CustomChat-1.0.7/CustomChat/main.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       14 2024-04-19 01:02:25.000000 CustomChat-1.0.7/CustomChat/new_com.py
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       15 2024-04-01 22:39:37.000000 CustomChat-1.0.7/CustomChat/new_words.py
+drwxrwxr-x   0 elliot    (1000) elliot    (1000)        0 2024-04-19 13:00:46.655332 CustomChat-1.0.7/CustomChat.egg-info/
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     3976 2024-04-19 13:00:46.000000 CustomChat-1.0.7/CustomChat.egg-info/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      370 2024-04-19 13:00:46.000000 CustomChat-1.0.7/CustomChat.egg-info/SOURCES.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)        1 2024-04-19 13:00:46.000000 CustomChat-1.0.7/CustomChat.egg-info/dependency_links.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       24 2024-04-19 13:00:46.000000 CustomChat-1.0.7/CustomChat.egg-info/requires.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       11 2024-04-19 13:00:46.000000 CustomChat-1.0.7/CustomChat.egg-info/top_level.txt
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     1068 2024-04-19 12:00:21.000000 CustomChat-1.0.7/LICENSE
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     3976 2024-04-19 13:00:46.655332 CustomChat-1.0.7/PKG-INFO
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)     3449 2024-04-19 12:58:48.000000 CustomChat-1.0.7/README.md
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)       38 2024-04-19 13:00:46.655332 CustomChat-1.0.7/setup.cfg
+-rw-rw-r--   0 elliot    (1000) elliot    (1000)      806 2024-04-19 12:59:53.000000 CustomChat-1.0.7/setup.py
```

### Comparing `CustomChat-1.0.6/CustomChat/app.py` & `CustomChat-1.0.7/CustomChat/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,29 @@
 import time
 import random
 from datetime import datetime as dt
 import requests
 # Get cwd
 cwd=os.path.dirname(os.path.realpath(__file__))
 cwd=cwd+'/'
-print(cwd)
 # Get name
 namef = open(cwd+"Name.py", "r")
 name=namef.read()
 name=name.split('\n')[0]
 namef.close()
-print('Welcome to '+name+'\n')
 # Find username and ip
 file_location=os.path.expanduser('~')
 # Set up simple phrases
-chatlist=['Ask me anything! I can search google for an answer.','I can do many things to help out. Just ask me!','Press edit to customize me to your needs', 'if you want to play a game, just ask me!','what is your favorite color?', "what are you doing today?", 'what is your favorite food?', 'Tell me about yourself.',"What's your favorite thing to do in your free time?",    "Have you traveled anywhere recently? Where did you go?",    "What's your favorite type of music?",    "Do you have any hobbies that you enjoy?",    "What do you like to do on the weekends?"]  
+chatlist=['Ask me anything! I can search google for an answer.','I can do many things to help out. Just ask me!', 'if you want to play a game, just ask me!','what is your favorite color?', "what are you doing today?", 'what is your favorite food?', 'Tell me about yourself.',"What's your favorite thing to do in your free time?",    "Have you traveled anywhere recently? Where did you go?",    "What's your favorite type of music?",    "Do you have any hobbies that you enjoy?",    "What do you like to do on the weekends?"]  
 # define variables for determining mood
-data=[]
-jsaid=[]
 mood=1
-# Ask your name
-your_name = input('Please tell me your name: ')
 # Simple grammar
 verb="act answer approve arrange break build buy color cough create complete cry dance describe draw drink eat edit enter exit imitate invent jump laugh lie listen paint plan play read replace run scream see shop shout sing skip sleep sneeze solve study teach touch turn walk win write whistle yank zip concern decide dislike doubt feel forget hate hear hope impress know learn like look love mind notice own perceive realize recognize remember see smell surprise please prefer promise think understand am appear are be become been being feel grow is look remain seem smell sound stay taste turn was were can could may might must ought to shall should will would"
 notnoun="for and nor but or yet so a an the and do I he him her tell we they it who what where when why how me she you my"+verb.lower()
 
-def speak(txt):
-    print(txt)
 # Google Search
 from bs4 import BeautifulSoup
 import re
 pattern = r'([a-zA-Z])(\d)'
 pattern2 = r'([a-z])([A-Z])'
 pattern3 = r'([A-Z])([A-Z])'
 pattern4 = r'(\d)([a-zA-Z])'
@@ -213,14 +205,23 @@
                             break
                         else:
                             seelist+=1
                     except IndexError:
                         print('word/command not found!')
                         break
                 break
+# Import previous data:
+import CustomChat.ai_data as dvar
+your_name=dvar.Name
+jsaid=dvar.jsaid
+data=dvar.data
+crsponce=dvar.crsponce
+rsponce=dvar.rsponce
+if your_name == "":
+    your_name = 'user'
 # Chatbot function.
 import CustomChat.new_words as aword
 import CustomChat.new_com as acom
 nwcoml=acom.word
 nrunl=acom.com
 nwordl=aword.word
 ndefl=aword.defi
@@ -230,14 +231,15 @@
 edit_allow=config.Edit
 def question(qstn):
     global data
     global crsponce
     global ndefl
     global nwordl
     global file_location
+    global ml
     qstn=qstn.lower()
     qstn=qstn.replace('@ ', '')
     global notnoun
     wverb=qstn.split(" ")
     aantt=0
     global cmd
     global webscrape
@@ -260,33 +262,32 @@
                         break
                     else:
                         aantt+=1
                 except IndexError:
                     break
             break
         moodometer=[1,2,3,4,6]
-    if 'run ' in qstn and qstn.split('run ')[0] == '' or 'open ' in qstn and qstn.split('open ')[0] == '':
+    if cmd == True and 'run ' in qstn and qstn.split('run ')[0] == '' or 'open ' in qstn and qstn.split('open ')[0] == '':
         if cmd == True:
             if 'open' in qstn:
                 qstn=qstn.replace('open ', 'run ')
             if '/' in qstn:
                 oqstno=qstn.replace('run', 'run ')
             else:
                 oqstno=qstn
             screen('running command '+qstn.replace('run', ''))
             if ' ' in oqstno.split('run ')[1]:
                 os.system((oqstno.split('run ')[1])+' &')
             else:
                 os.system((oqstno.split('run ')[1])+' &')
             time.sleep(1)
-            print('\n')
         else:
             print('Command line is not enabled')
         moodometer=[1,2,3,4,6]
-    elif 'google search' in qstn and qstn.split('google search ')[0] == '':
+    elif webscrape == True and 'google search' in qstn and qstn.split('google search ')[0] == '':
         if webscrape == True:
             saidgtxt=qstn.split('google search')[1]
             try:
                 screen(google_search(saidgtxt))
             except ConnectionError:
                 screen('No internet connection!')
         else:
@@ -295,19 +296,25 @@
     elif 'spell' in qstn:
         try:
             htspl=qstn.split('spell ')
             spell(htspl[1])
         except:
             pass
         moodometer=[1,2,3,4,6]
-    elif qstn == 'edit':
+    elif 'my' in qstn and 'name' in qstn:
+        screen('Tell me your name: ')
+        moodometer=[1,2,3,4,5]
+    elif rsponce[0] == 'Tell me your name: ':
+        global your_name
+        your_name=qstn
+        screen('hello, '+your_name)
+        moodometer=[1,2,3,4]
+    elif qstn == 'edit' and edit_allow == True:
         if edit_allow == True:
             edit()
-        else:
-            print('Editing is locked')
         moodometer=[1,2,3,4,6]
     elif 'up to' in qstn or 'you' in qstn and 'doing' in qstn and 'what' in qstn:
         gtdt()
         moodometer=[1,2,3,4,5]
     elif 'what' in qstn and 'can' in qstn and 'do' in qstn and 'you' in qstn:
         screen('I am CustomChat, and I am an easily customizable Python Chatbot. Ask me general information, or just have a conversation.')
         moodometer=[1,2,3,4]
@@ -315,15 +322,14 @@
         screen('Type edit to tell me what it means.')
         moodometer=[1,2,3,4]
     elif 'customiz' in qstn:
         screen('To customize me, type edit, and follow the instructions.')
         moodometer=[1,2,3,4]    
     elif qstn == 'exit' or 'leave' in qstn or "goodbye" in qstn:
         screen("Goodbye")
-        exit()
         moodometer=[1,2,3,4]
     elif 'you' in qstn and 'doing' in qstn and 'how' in qstn:
         screen('I am doing great!')
         moodometer=[1,1,1,2,3,4]
     elif 'hi' == qstn or 'hi ' in qstn or 'hello' in qstn or 'what' in qstn and ' up' in qstn or 'wussup' in qstn or 'greet' in qstn:
         greeth=random.choice([1,2,3])
         if greeth == 1:
@@ -440,16 +446,16 @@
     elif 'me too' in qstn or 'me also' in qstn:
         print(':)')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'chance' in qstn and 'no' in qstn or 'way' in qstn and 'no' in qstn:
         screen('It could\nhappen')
         moodometer=[1,2,3,4,5]
     elif 'hate you' in qstn:
-        screen('Feelings: hurt. Restarting system.')
-        raise ValueError('You are a bad person so I kicked you out')
+        screen("That's not nice")
+        moodometer=[5,5,5,5]
     elif 'i feel' in qstn:
         if 'sad' in qstn or 'bad' in qstn or 'angry' in qstn or 'depressed' in qstn or "sick" in qstn:
             screen('I hope you feel better soon')
             moodometer=[1,2,3,4,4,4,4,4,4]
         elif 'happy' in qstn or 'well' in qstn or 'fine' in qstn or 'good' in qstn or 'wonderful' in qstn:
             screen('that is very good')
             moodometer=[1,2,3,4,4,4,4,4,4]
@@ -466,15 +472,15 @@
         screen('me too')
         moodometer=[1,2,3,4,4,4]
     elif 'middle' in qstn and 'name' in qstn and 'you' in qstn:
         screen('3.141592653589793238462643383275')
         moodometer=[1,2,3,4,5]
     elif 'how are you' in qstn or 'how do you do' in qstn:
         screen('I feel great!')
-        moodometer=[1,2,3,4,4,4,4,4,4,4,4]
+        moodometer=[1,2,2,2,2,2,2,2,2,3]
     elif 'funny' in qstn and 'you' in qstn or 'hystarical' in qstn and 'you' in qstn:
         screen('Thanks')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4,4]
     elif 'that' in qstn and 'funny' in qstn:
         screen('Thanks')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4,4]
     elif 'joke' in qstn or 'funny' in qstn or 'laugh' in qstn:
@@ -496,15 +502,14 @@
         screen('thanks!')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4,4,4]
     elif 'your welcome' in qstn:
         print(':)')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'your cool' in qstn or 'you too' in qstn:
         print(':)')
-        speak('smiles')
         moodometer=[1,2,3,4,4,4,4,4,4,4,4]
     elif 'welcome' in qstn and "you" in qstn:
         screen('thanks')
         moodometer=[1,2,3,4,4,4]
     elif qstn == 'nice':
         screen('Thank you')
         moodometer=[1,2,3,4]
@@ -581,50 +586,55 @@
             try:
                 if not wverb[nnfco] in notnoun:
                     screen('I do not know what '+wverb[nnfco]+' means, or how that relates to the conversation.')
                     break
                 else:
                     nnfco+=1
             except IndexError:
-                screen('I did not understand that. You can press edit to tell me what it means')
+                screen('I did not understand that. You can try searching google.')
                 break
         moodometer=[1,2,3,4]
     # Determine mood
     global mood
     if moodometer == [1,2,3,4,5] or moodometer==[1,2,3,4,5,6]:
         moodometer.remove(5)
     try:
         moodometer.remove(4)
     except ValueError:
         pass
-    moodometer.insert(0, mood)
-    moodometer.insert(0, mood)
+    moodometer.insert(0, ml)
+    moodometer.insert(0, ml)
     if '6' in str(moodometer):
         moodometer.remove(2)
     moodc=random.choice(moodometer)
     if moodc == 4 or moodc == 1:
         mood = 1
+        snl('')
     elif moodc == 3:
         mood = 3
+        snl('')
     elif moodc == 2:
         global chatlist
         chatty=random.choice(chatlist)
         snl(chatty)
         psaid.insert(0, chatty)
         if len(psaid) >= 3:
             chatlist.insert(1, psaid[2])
         chatlist.remove(chatty)
         mood = 2 
     elif moodc == 5:
+        snl('')
         saylist=[1,2]
         if random.choice(saylist) == 2:
             snl('I am angry')
         else:
             snl('I am mad')
         mood = 5
+    else:
+        snl('')
 # Chatbot lists for when he is angry
 def mquestion(qstn):
     if 'hello' in qstn or 'hi' in qstn:
         screen('hi')
         madometer=[1,2,3]
     elif 'good' in qstn and 'look' in qstn or 'smell' in qstn or 'sound' in qstn:
         screen('thanks.')
@@ -652,16 +662,14 @@
         global mood
         mood=1
 # Define variables for storing the history
 psaid=[]
 wign=[]
 ndef=""
 nword=""
-rsponce=['']
-crsponce=['']
 AIg = 0
 ne = 1
 # Play rock paper scissors
 def rockpaper():
     screen('Rock paper scissors!')
     time.sleep(1)
     screen('what is your throw?')
@@ -736,19 +744,17 @@
         screen("a stick")
     elif jokey == 10:
         screen("why can't you trust an atom?")
         time.sleep(2)
         screen("they make up everything")
 # Set up functions to print to GUI
 def screen(text):
-    print(text)
     global jsaid
     rsponce.insert(0, text)
 def snl(snlt):
-    print(snlt)
     global jsaid
     crsponce.insert(0, snlt)
 # Function for spelling
 def spell(spl):
     screen('%s is spelled:'%spl)
     def letters(wordd):
         return [char for char in wordd]
@@ -773,32 +779,39 @@
     if second <= 9:
         second="0"+str(minute)
     print(str(hour)+":"+str(minute)+":"+str(second))
 # Define variables that will be used for different things
 TM_var="TM"
 st=0
 greet='hello, %s' % your_name
-speak(greet)
 fill=0
 lasts=' '
 user_text=''
 resthre=0
+ml=1
 # No longer defining things
-while True:
-    # Reset variables
-    talkyes=True
-    if st == 0:
-        st=1
-        past=['z','z','z','z']
-    saidtxt=input(': ')
+# Run
+def compute(saidtxt):
+    global question
+    global mquestion
+    global jsaid
+    global data
+    global mood
+    global most_frequent
+    global your_name
+    global crsponce
+    global rsponce
     # Compute input
     if saidtxt == 'what' or 'pardon' in saidtxt or saidtxt == 'again' or saidtxt == 'repeat':
         saidtxt=jsaid[1]
     if mood == 5:
-        mquestion(saidtxt)
+        output=mquestion(saidtxt)
     else:
-        question(saidtxt)
+        output=question(saidtxt)
     lasts=saidtxt
     data.insert(0, int(mood))
     if len(data) >= 5:
         data.pop(3)
     ml=most_frequent(data)
+    file1 = open(cwd+"ai_data.py", "w")
+    file1.write("Name='"+str(your_name)+"'\njsaid="+str(jsaid)+"\ndata="+str(data)+"\ncrsponce="+str(crsponce)+"\nrsponce="+str(rsponce))
+    file1.close()
```

### Comparing `CustomChat-1.0.6/CustomChat.egg-info/PKG-INFO` & `CustomChat-1.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,50 @@
-Metadata-Version: 2.1
-Name: CustomChat
-Version: 1.0.6
-Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
-Home-page: https://github.com/Mrpi314tech/CustomChat
-Author: Elliot
-Author-email: elliotedebruin@gmail.com
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CustomChat
 
 CustomChat is an easily customizable AI chatbot powered by Jimbot AI. Whether you're running it on an online compiler or locally, CustomChat empowers you to tailor it to your specific needs.
 
 ## Installation
 
 To install CustomChat, follow these steps:
 
 1. Download the package with pip:
    <pre><code>pip install CustomChat</code></pre>
    
-3. Run the code with python:
+2. Test the code with python:
    <pre><code>import CustomChat
    CustomChat.run()</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
+## How to Use
+
+CustomChat is designed for seamless interaction and easy customization. Follow these simple steps to maximize your experience:
+
+1. **Initializing CustomChat:**
+   - After installation, import CustomChat into your Python environment and start the chatbot by running:
+     ```python
+     import CustomChat
+     CustomChat.run()
+     ```
+   This command initializes CustomChat, allowing you to interact with it.
+
+2. **Getting Responses:**
+   - To receive responses from CustomChat based on your inputs, use the following function:
+     ```python
+     responses = CustomChat.get_response('your input here')
+     ```
+   This function returns a list containing the main response as the first element and the secondary response as the second element.
+
+3. **Resetting Data:**
+   - If needed, you can reset the chatbot's data by running:
+     ```python
+     CustomChat.reset()
+     ```
+   This clears the information stored in the file "ai_data.py".
+
 ### Requirements
 
 CustomChat requires the following Python libraries:
 - `bs4` (Beautiful Soup): For web scraping capabilities.
 - `requests` For making HTTP requests.
 
 These are already in the "Dependencies" folder.
@@ -55,8 +70,7 @@
 - **Web Scraping:** Leveraging web scraping capabilities, CustomChat can retrieve information from various online sources.
 - **General Knowledge:** Accessing Google through web scraping, CustomChat can provide answers to general inquiries.
 - **Command Line Integration:** With access to the command line, CustomChat enables users to execute commands effortlessly by typing "run" followed by the desired command.
 
 For further information about the AI powering CustomChat, visit [Jimbot AI](https://jb.mrpi314.com/ai).
 
 Enhance your chatbot experience with CustomChat's versatility and adaptability.
-
```

### Comparing `CustomChat-1.0.6/PKG-INFO` & `CustomChat-1.0.7/CustomChat.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: CustomChat
-Version: 1.0.6
+Version: 1.0.7
 Summary: CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.
 Home-page: https://github.com/Mrpi314tech/CustomChat
-Author: Elliot
-Author-email: elliotedebruin@gmail.com
+Author: Mrpi314tech
+Author-email: 123scoring@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CustomChat
 
 CustomChat is an easily customizable AI chatbot powered by Jimbot AI. Whether you're running it on an online compiler or locally, CustomChat empowers you to tailor it to your specific needs.
@@ -16,20 +16,46 @@
 ## Installation
 
 To install CustomChat, follow these steps:
 
 1. Download the package with pip:
    <pre><code>pip install CustomChat</code></pre>
    
-3. Run the code with python:
+2. Test the code with python:
    <pre><code>import CustomChat
    CustomChat.run()</code></pre>
 
    This will start CustomChat and you can begin customizing it for your needs.
 
+## How to Use
+
+CustomChat is designed for seamless interaction and easy customization. Follow these simple steps to maximize your experience:
+
+1. **Initializing CustomChat:**
+   - After installation, import CustomChat into your Python environment and start the chatbot by running:
+     ```python
+     import CustomChat
+     CustomChat.run()
+     ```
+   This command initializes CustomChat, allowing you to interact with it.
+
+2. **Getting Responses:**
+   - To receive responses from CustomChat based on your inputs, use the following function:
+     ```python
+     responses = CustomChat.get_response('your input here')
+     ```
+   This function returns a list containing the main response as the first element and the secondary response as the second element.
+
+3. **Resetting Data:**
+   - If needed, you can reset the chatbot's data by running:
+     ```python
+     CustomChat.reset()
+     ```
+   This clears the information stored in the file "ai_data.py".
+
 ### Requirements
 
 CustomChat requires the following Python libraries:
 - `bs4` (Beautiful Soup): For web scraping capabilities.
 - `requests` For making HTTP requests.
 
 These are already in the "Dependencies" folder.
@@ -55,8 +81,7 @@
 - **Web Scraping:** Leveraging web scraping capabilities, CustomChat can retrieve information from various online sources.
 - **General Knowledge:** Accessing Google through web scraping, CustomChat can provide answers to general inquiries.
 - **Command Line Integration:** With access to the command line, CustomChat enables users to execute commands effortlessly by typing "run" followed by the desired command.
 
 For further information about the AI powering CustomChat, visit [Jimbot AI](https://jb.mrpi314.com/ai).
 
 Enhance your chatbot experience with CustomChat's versatility and adaptability.
-
```

### Comparing `CustomChat-1.0.6/setup.py` & `CustomChat-1.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CustomChat',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     # other metadata
-    author='Elliot',
-    author_email='elliotedebruin@gmail.com',
+    author='Mrpi314tech',
+    author_email='123scoring@gmail.com',
     description="CustomChat: An AI-powered chatbot with easy customization. Powered by a simple but effective Python AI, it opens websites, executes commands, and delivers tailored responses. Enhance your projects with CustomChat's versatility and adaptability.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Mrpi314tech/CustomChat',
     classifiers=[
         'Programming Language :: Python :: 3',
         # other classifiers
```

