# Volla OS Guide

The Volla OS operating system and its special user interface are under continuous development. An overview of the development status can be found on the platform Github, where we publish the source code of the operating system. 

https://github.com/HelloVolla/

In the repository [volla-os-beta-test](https://github.com/HelloVolla/volla-os-beta-test) you can find this guide as well as the possibility to report bugs and track their fixes. 

https://github.com/HelloVolla/volla-os-beta-test/issues

Unlocking a Volla Phone with a Volla OS operating system will take you to the Volla Launcher, which you can use to perform basic device functions including opening apps. 

You can also reach the Volla Launcher by pressing the Home button at the bottom of the display or by making the corresponding swipe gesture from the bottom outside of the display to the inside.

Hiding the Android navigation bar completely is done for Volla Launcher in its settings in the "Display and menus" group by tapping "Full screen view". You can get to the Volla Launcher settings by swiping to the right twice, so that the settings appear from the left side.

The Volla user interface includes two basic concepts:

1. springboard with
	2. text field and
	3. shortcuts
3. collections for
	4. contacts
	5. conversations
	6. messages
	7. notes

## Springboard

Whenever you open the Volla Launcher, it shows the springboard. The idea is that you write something and the system recognizes what you want to. In return it provides suggestions to complete your input or suitable functions for your input.

![Springboard](screenshot-springboard.jpeg)

Springboard supports the following use cases:

### Contact selection
When you start typing with the @ sign, the system recognizes that you want to enter a name and suggests people from the address book, tentatively sorted by name. If you tap on a name in the list, it will be taken over in the text field. Prerequisite for this function is that there are entries in your address book.

By entering further letters you can filter the list of contacts. Here the springboard shows the names that contain the entered letter sequence at any position.

For example, you can synchronize contacts with the installed app for synchronizing address books and calendars using the CardDAV and CalDAV protocols.

### Call
Then the system will suggest that you call this person. When you tap on the suggestion for this function, the system will start a call via the Telephony app. You can recognize suggestions for functions by the red background color, unlike suggestions for completing your input.

	@Claudia_Sommer

### Messages
If you enter more words instead of making a call, the system suggests that you can send a text message or email to the contact you entered. If you tap on the suggestion, the app will open the respective app with a pre-filled message, which you only have to send. 

	@Claudia Sommer Will you come with us to the Italian restaurant during lunch break?

If you use a line break after the words, the system uses the first line for the subject of an email. The requirement is that you have created at least one email account.

	@Claudia_Sommer Lunch break
	Would you like to go to the Italian restaurant with us during the lunch break?
	Greetings from Petra
	
Depending on the data stored for a contact, Volla Launcher suggests sending a message as SMS, email via Signal Messenger service.  

### Web search
If you start the input instead of a word instead of a contact, the system suggests to search the Internet with this word. For this purpose, the system starts the browser with the entered keyword. By default, Volla Launcher uses the [DuckDuckGo](https://duck.com) search engine. In the settings, you can also select [Starpage](https://startpage.com) or [Metager](https://metager.de) in the "Search engines" group.

	Volla
	
### Note
If you enter several words, the system also suggests that you can create a note. You will then find this as an entry in the collections for notes via the red dot.

	Fulla Phone
	
You can also use line breaks.

	Volla Phone
	New features:
	1. security mode
	2. mult boot
	
### Web address
When you enter a valid web address, the system suggests to open it in the browser.

	volla.online
	
### Phone number
If you enter a phone number in the text field, the system will suggest you to make a call. As with all inputs, a space at the end of a word or a sequence of digits is necessary to trigger the evaluation of the input.

	014323566777
	
If you then enter one or more words, the system will offer to send a text message, but not an e-mail.

	014323565777 Hello Petra, how are you?
	
### E-mail address

If you enter an email address and a text, Volla Launcher suggests sending an email. 

	hello@volla.online Where can I buy a Volla Phone?  
	
If you enter several times, the first line will be used as the subject of the email:
	
	hello@volla.online Volla retailer
	Dear Volla team,
	Where can I buy a Volla Phone? 	

### Calendar event

Volla Launcher recognizes different forms of calendar event description which consists of date, optional time, title and optional description. 

	08/12/2022 12:00 Lunch with Peter
	12.08. 16:30 - 17:30 Training at the sports club
	6 - 8 pm Dinner with Paula at Joe's Pizzaria.  

If the time is missing, the Volla Launcher will schedule a day event. Error only the second time for the event. If the date is missing, the same day applies. 

Instead of a date, you can also choose days of the week or a short form:

	Tomorrow 10 am video conference with Paula
	Thursday 14 - 18 o'clock wine seminar in the Ratskeller 

In case of a line break, Volla Launcher uses the text after the first line break as a description of the calendar event. 

When you tap on the suggestion to add the event to the calendar, the system opens the Calendar App where you confirm the event to send it off.
	
More use cases are planned.

## Shortcuts

On the springboard you can see a red dot. With diem you call shortcuts with just one gesture. To do this, touch the dot so that the menu opens, slide your finger or stylus over the desired menu item and lift your finger or stylus:

1. touch
2. slide
3. release

![Shortcuts](sceenshot-shortcuts.jpeg)

The default contains the following functions:

- Calling recent and favorite contacts
- Calling recent conversations
- Calling recent messages
- Calling notes
- Calling the phone app
- Calling the camera
- Calling the gallery
- Calling the calendar app

You can manage the shortcuts in the settings under the corresponding group of Volla Launcher. You can disable and enable default functions, while you can also delete self-defined shortcuts. 

You can add new shortcuts in two ways:

1. tap and hold on an app in the overview until a context menu appears and select the "Add to shortcuts" option.
2. Swipe right twice from the springboard to bring up the settings from the left. Tap on the "Shortcuts" group and then on the plus sign to open a context menu from which you can select ine app. 

A tip: You can also add Internet addresses that you have bookmarked in the app overview to the shortcuts using this method. 

## Collections

Collections give you a quick overview of important information and matching functions. After calling a collection, you will see an animation with which the system shows the collection from the right side.

You can navigate back to the springboard with a swipe gesture, the home button or the home gesture. 

You can filter each collection using a text field under the heading.

### Contacts
The system automatically compiles important contacts. In the beta version, the system takes into account all contacts that you have marked as a favorite in the address book or with whom you have recently been in contact via a phone call or an SMS or MMS message.

In the contacts overview, you can find the contact's name as well as its organization or the most recent unread message or missed call. 

If you tap and hold an entry for a short time, the system opens a context menu and offers the following functions depending on the address book entry: 

- Calling the address book entry
- Call of the signal profile
- Start a call
- Calling the Messenger app to write and send a text message
- Calling the e-mail app to write and send an e-mail

Again, the selection is made according to the shortcut gesture.

If you just briefly tap on an entry, the system opens the conversation with the person, which for the time being includes calls, SMS and MMS messages.

At the bottom of the view, you will find a text field that allows you to reply directly via SMS or MMS. 

Signal message integration is in preparation. 

### Conversations
Here the system displays the most recent conversations with name or phone number and text, which it sorts by time and topic. The beta version takes SMS and MMS messages into account. Other communication channels are planned.

If you briefly tap on a conversation, the system shows the conversation with all exchanged messages.

Again, you can reply directly via SMS, MMS and in the future via the Signal Messenger service using the text box at the bottom

### Messages
Here the system shows recent messages grouped by their source and sorted by time. This has the advantage that important messages from sources that publish messages less frequently do not get lost in the message stream. 

Tapping the news channel icon will take you to all the recent publications of that selected news channel. 

On the other hand, if you tap on the displayed news, you will get to the full news, which the system edits for optimal readability.

By default, Volla Launcher shows the RSS feed of three news channels as an example. You can subscribe to your own RSS or Atom feeds from news portals and blogs in two ways: 

1. tap and hold a link to an RSS or Atom news feed in the browser until a context menu appears. Select the option to share the link with Volla Launcher. 
Write or copy the link to an RSS or Atom news feed into the text field of the springboard. Springboard will suggest you to subscribe to this feed. 

In the Volla Launcher settings you can disable and enable news feeds in the News Channels group, or delete them completely by tapping the cross in the right margin. 

### Notes
In this collection, Volla Launcher lists all the notes you have created either from the springboard or from the list view of this collection.

Tap on a list entry to read the full note. In the details view, you can edit, delete, or pin a note to the top of the list. Pinned notes can also be unpinned using the same method. 

Links with or without protocol prefix and lists are automatically recognized and formatted by Volla Launcher.

	A list
	1, Sorted lists
	- Unsorted lists
	* Various bullets

## Apps

If you swipe right from the springboard, you will get to the overview of installed apps, sorted in alphabetical order of names.

By default, the apps are divided into two groups: Frequently used apps and other apps. Using the Volla Launcher settings, you can also display the apps ungrouped or in additional groups, one for each app category. 

Regardless of grouping, you can filter the apps displayed using the text box.

A red dot indicates if you missed a call or haven't read a text message yet.

## Settings

If you swipe right from the app grid, you will get to the app's settings. 

The first group you will find is the selection of the design theme. 

- Dark mode
- Light mode
- Transparent mode

The transparent mode uses the background image that you can change in the system settings. Changing the design mode also defines the lock screen background image at the same time. 

## Standard Apps

The Full OS comes without Google Apps and Play Services to protect user privacy. Therefore, it contains curated, open-source alternatives. See also the corresponding overview. 

https://github.com/HelloVolla/volla-os-beta-test/wiki/Curated-Pre-Installed-System-Apps

To selection is not final yet. 

## Miscellaneous

This document will also be revised. General questions and suggestions are welcome via our contact form or via the Volla Beta Testers group on Telegram:

https://volla.online/de/contact/

For invitation to the Telegram group for beta testers, please email Marc Aurel with the address @m_aurel.