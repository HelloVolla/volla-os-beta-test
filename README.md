# Volla OS Beta Guide

The beta version of the Full OS is still incomplete and contains bugs. An overview of the development status can be found on the platform Github, where we publish the source code of the operating system. 

https://github.com/HelloVolla/

In the repository [volla-os-beta-test](https://github.com/HelloVolla/volla-os-beta-test) you will find this manual as well as the possibility to report bugs and track their resolution. 

https://github.com/HelloVolla/volla-os-beta-test/issues

If you unlock the Volla Phone with a Volla OS operating system, you will get to the Volla Launcher, which allows you to perform the basic functions of the device including opening apps. 

You can also access the Volla Launcher by clicking the Home button at the bottom of the display or by using the appropriate wiping gesture from the bottom outside of the display to the inside.

The complete hiding of the Android navigation bar is not yet implemented in the beta version of the Volla OS.

The Volla user interface comprises two basic concepts:

1. springboard with
	2. text field and
	3. shortcuts
3. collections for
	4. contacts
	5. conversations
	6. news

## Springboard

Whenever you call the Volla Launcher, it shows the springboard. The idea is that you write something and the system recognizes what you want to do. To do this, it provides suggestions for completing your input or suitable functions for your input.

![Springboard](screenshot-springboard.jpeg)

The springboard supports the following use cases:

### Contact selection
When you start typing with the @ sign, the system recognizes that you want to type a name and suggests people from the Address Book, tentatively sorted by name. If you tap a name in the list, it will be applied in the text field. A prerequisite for this function is that there are entries in your address book.

For example, you can synchronize contacts with the installed app for synchronizing address books and calendars via the CardDAV and CalDAV protocol.

### Call
The system then suggests that you call this person. If you tap the proposal for this function, the system calls the telephony app. Unlike proposals for completing your entry, you can recognize proposals for functions by the red background color.

	@Claudia_Summer

### Messages
If you enter more words instead of triggering a call, the system suggests that you can send a text message or e-mail to the contact you entered. If you tap on the suggestion, the app currently opens the respective app with a pre-filled message that you only need to send. 

	@Claudia Sommer Will you come with us to the Italian restaurant during the lunch break?

If you use a line break after the words, the system uses the first line for the subject of an e-mail. Prerequisite is that you have created at least one e-mail account.

	@Claudia_Summer Lunch Break
	Would you like to join us for an Italian meal during your lunch break?
	Greetings from Petra

### Web search
If you start typing instead of a word instead of a contact, the system will suggest that you search the Internet with that word. To do this, the system starts the browser with the keyword you entered. Currently the beta version uses the search engine DuckDuckGo. It is planned to select a search engine in the settings.

	Volla
	
### Note
If you enter several words, the system also suggests that you can create a note. For the time being, the beta version creates a text file, which you can find in the document directory with the app for displaying your files, and which you can open and edit again with the app for notes. 

	Volla Phone
	
You can also use line breaks
	
### Web address
If you enter a valid Internet address, the system suggests opening it in the browser.

	volla.online
	
### Phone number
If you enter a phone number in the text field, the system will also suggest that you initiate a call. In the beta version, as with all entries, a space at the end of a word or a sequence of digits is required to trigger the evaluation of the entry.

	014323566777
	
If you then enter one or more words, the system will offer to send a text message, but you will still receive an e-mail.

	014323565777 Hello Petra, how are you?
	
More use cases are planned.

## Shortcuts

On the springboard you can see a red dot. With diem you call up shortcuts with just one gesture. To do this, touch the dot so that the menu opens, slide your finger or stylus over the desired menu item and lift your finger or stylus:

1. Touch
2. Drag
3. Release

![Shortcuts](sceenshot-shortcuts.jpeg)

The beta version supports fixed functions:

- Calling of important contacts
- Calling up the latest conversations
- Recent news retrieval
- Calling the Calendar App
- Calling the Phone App
- Calling the camera

The selection of the desired shortcuts is planned in the settings.

## Collections

The collections give you a quick overview of important information and suitable functions. After calling up a collection, you will see an animation with which the system displays the collection from the right side.

You can use a wipe gesture, the Home button or the Home gesture to navigate back to the springboard. 

You can filter each collection using a text box under the heading.

### Contacts
The system automatically compiles important contacts. In the beta version, the system will take into account all contacts that you have marked as favourites in the address book or with whom you have recently been connected via a phone call or an SMS or MMS message.

In the overview of contacts you will find the name of the contact and its organization or the latest unread message or a missed call. 

Tap on an entry and hold the touch for a short time, the system opens a context menu and offers, depending on the address book entry, functions for a call, a text message or an e-mail. Here too, the selection is made according to the gesture for shortcuts.

If you tap an entry for a short time, the system opens the conversation with the person temporarily containing calls, SMS and MMS messages.

A direct reply in the conversation is planned.

### Conversations
Here the system displays the most recent conversations with name or phone number and text, which it sorts by time and topic. The beta version includes SMS and MMS messages. Further communication channels are planned.

If you briefly tap on a conversation, the system displays the conversation with all messages exchanged.

### Messages
Here the system displays the latest news grouped by source and sorted by time. This has the advantage that important news from sources that publish news less frequently is not lost in the news stream. 

If you tap on the symbol of the news channel, the system displays all the latest publications of this selected news channel. 

If you tap on the displayed message, however, you will be taken to the complete message, which the system prepares for optimal readability.

The beta version takes the RSS feed of three news channels into account as an example. It is planned to provide self-selected RSS feeds and other news channels such as Twitter.

## Apps

If you make a wiping gesture to the right from the springboard, you will get to the overview of installed apps, which the system sorts alphabetically by name in the beta version. 

Here you can also filter the displayed elements with a text field.

A red dot indicates whether you missed a call or did not read a text message.

## Settings

If you make a wiping gesture to the right from the app grid, you can access the app's settings. 

The first beta version only supports the selection of the design theme. 

- Dark Mode
- Bright mode
- Translucent mode

The trnalucent mode uses the background image that you can change in the system settings.

## Standard Apps

The Volla OS comes without Google Apps and Play Services to protect the privacy of users. Therefore it contains curated, open source alternatives. See also the corresponding overview. 

https://github.com/HelloVolla/volla-os-beta-test/wiki/Curated-Pre-Installed-System-Apps

Selection is not yet final. 

## Miscellaneous

This document will also be revised. General questions and suggestions are welcome via our contact form or via the Volla Beta-Tester Group on Telegram:

https://volla.online/contact-form/

For the invitation to the Telegram Group for the beta testers, please write to Marc Aurel at the address @m_aurel.

Translated with www.DeepL.com/Translator (free version)l

The beta version supports fixed functions:

- Calling of important contacts
- Calling up the latest converters
- Recent news retrieval
- Calling the Calendar App
- Calling the Phone App
- Calling the camera

The selection of the desired shortcuts is planned in the settings.

## Collections

The collections give you a quick overview of important information and suitable functions. After calling up a collection, you will see an animation with which the system displays the collection from the right side.

You can use a wipe gesture, the Home button or the Home gesture to navigate back to the springboard. 

You can filter each collection using a text box under the heading.

### Contacts
The system automatically compiles important contacts. In the beta version, the system will take into account all contacts that you have marked as favourites in the address book or with whom you have recently been connected via a phone call or an SMS or MMS message.

In the overview of contacts you will find the name of the contact and its organization or the latest unread message or a missed call. 

Tap on an entry and hold the touch for a short time, the system opens a context menu and offers, depending on the address book entry, functions for a call, a text message or an e-mail. Here too, the selection is made according to the gesture for shortcuts.

If you tap an entry for a short time, the system opens the conversation with the person temporarily containing calls, SMS and MMS messages.

A direct reply in the conversation is planned.

### Conversations
Here the system displays the most recent conversations with name or phone number and text, which it sorts by time and topic. The beta version includes SMS and MMS messages. Further communication channels are planned.

If you briefly tap on a conversation, the system displays the conversation with all messages exchanged.

### Messages
Here the system displays the latest news grouped by source and sorted by time. This has the advantage that important news from sources that publish news less frequently is not lost in the news stream. 

If you tap on the symbol of the news channel, the system displays all the latest publications of this selected news channel. 

If you tap on the displayed message, however, you will be taken to the complete message, which the system prepares for optimal readability.

The beta version takes the RSS feed of three news channels into account as an example. It is planned to provide self-selected RSS feeds and other news channels such as Twitter.

## Apps

If you make a wiping gesture to the right from the springboard, you will get to the overview of installed apps, which the system sorts alphabetically by name in the beta version. 

Here you can also filter the displayed elements with a text field.

A red dot indicates whether you missed a call or did not read a text message.

## Settings

If you make a wiping gesture to the right from the app grid, you can access the app's settings. 

The first beta version only supports the selection of the design theme. 

- Dark Mode
- Bright mode
- Transparent mode

The transparent mode uses the background image that you can change in the system settings.

## Standard Apps

The Volla OS comes without Google Apps and Play Services to protect the privacy of users. Therefore it contains curated, open source alternatives. See also the corresponding overview. 

https://github.com/HelloVolla/volla-os-beta-test/wiki/Curated-Pre-Installed-System-Apps

Selection is not yet final. 

## Miscellaneous

This document will also be revised. General questions and suggestions are welcome via our contact form or via the Volla Beta-Tester Group on Telegram:

https://volla.online/contact-form/

For the invitation to the Telegram Group for the beta testers, please write to Marc Aurel at the address @m_aurel.