# OFFLINE-BOT — Offline Guild Official Bot

OFFLINE-BOT is the **official Discord bot for Offline Guild**, an online gaming guild focused on **MMO (Massively Multiplayer Online) games**.

The bot was created to help manage guild activities, announcements, parties, and member interactions through Discord. It also includes an **AI assistant** that can answer questions through both text and voice channels.

## AI Assistant

One of the main features of OFFLINE-BOT is its AI assistant.

Members can ask questions through a Discord text channel, and the AI can respond directly in the channel.

The bot can also interact through voice channels. Members can join a voice channel and use the wake-up call **"Offline"** followed by their question. The bot listens to the question, processes it with the AI, and speaks the response out loud.

The bot can also **read announcements aloud** when their scheduled announcement time is reached.

## Guild-Manager Integration

OFFLINE-BOT is connected to **Guild-Manager**, a separate web-based management system that provides a UI for managing guild activities.

Guild-Manager can be used to:

* Create and manage announcements
* Create parties
* Manage other guild-related activities

Announcements and other actions can also be managed directly through OFFLINE-BOT's Discord commands.

## Announcement System

OFFLINE-BOT includes a scheduled announcement system for the guild.

All announcement data is stored in a **MongoDB Atlas backend**. Admins can create announcements through the bot or through **Guild-Manager**.

Each announcement contains its scheduled date and other required information. When the scheduled time is reached, OFFLINE-BOT automatically sends the announcement.

For voice channels, the bot can also **speak the announcement out loud**, allowing guild members to hear scheduled announcements without needing to check the text channel.

Admins can also cancel announcements using their announcement ID.

## Discord Commands

### `/announce`

Allows an admin to create an announcement.

### `/announcements`

Displays the current active announcements, including their scheduled announcement dates.

The announcement list is only visible to the user who runs the command.

### `/cancelannounce`

Allows an admin to cancel an announcement using its announcement ID.

### `/clearchat`

Clears the AI's conversation history for the chat so that the AI no longer uses the previous conversation when answering new questions.

### `/join`

Makes the bot join the user's current voice channel and start listening.

### `/leave`

Makes the bot leave the voice channel.

### `/listen`

Allows the bot to listen to a specific Discord channel selected by the user and answer questions asked there using the AI.

### `/partydisplay`

Displays the current party list.

### `/unlisten`

Stops the bot from listening to the selected channel for AI questions.

### `/voicepanel`

Displays the voice control panel, including the mute and on/off controls.

## Technologies Used

* Discord Bot API
* AI / LLM Integration
* Voice Recognition
* Text-to-Speech
* JavaScript
* MongoDB Atlas
* Guild-Manager API / Backend
* Discord Voice Channels

## Project Purpose

OFFLINE-BOT was created to provide Offline Guild with a central Discord bot for handling guild activities and communication.

The project combines several features I wanted to experiment with, including AI conversations, voice recognition, text-to-speech, scheduled announcements, Discord interactions, and integration with a separate web-based management system.

It also became a practical project because the bot is actually used by the guild rather than being created only as a prototype.

## Project Status

**Currently Running and In Development**

OFFLINE-BOT is currently being used by Offline Guild.

The project is still actively being worked on, with ongoing improvements, fixes, and new features being added over time.

The bot is connected to the **Guild-Manager** project, which provides a web-based UI for managing guild activities alongside the Discord bot.
