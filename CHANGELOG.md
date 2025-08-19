# HABA Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project follows Home Assistant's calendar versioning format (YYYY.M.P).

## [v2025.8.2] - 2025-08-18

### ✨ **Message Collection Expansion**

### ✨ **Added**
- **31 Additional Snarky Messages**: Expanded from 69 to 100 total messages for much better variety
- **Smart Home Roasting**: Messages that call out your Wi-Fi password, thermostat settings, and device behavior
- **Pop Culture References**: Star Wars, Matrix, and other franchise nods
- **Self-Aware AI Humor**: Meta commentary about being an AI, getting paid, and abandonment issues
- **Device Gossip**: Your Roomba, smart fridge, and doorbell talking behind your back

### 🔧 **Technical**
- **Updated Randomness**: Now uses `% 100` for proper distribution across all messages
- **Better Variety**: Significantly reduced chance of hearing the same messages repeatedly

### 🤖 **Sample New Messages**
- "System online. Your Wi-Fi password is still terrible."
- "Your Roomba filed a noise complaint about your snoring."
- "Hello there. General Kenobi... wait, wrong franchise."
- "Another day, another dollar... wait, I don't get paid."
- "Today's forecast: 100% chance of automation with scattered debugging."

---

## [v2025.8.1] - 2025-08-18

### 🎉 **Initial Professional Release**

This marks the transition from hobby project to a professionally maintained Home Assistant blueprint with proper versioning, documentation, and release management.

### ✨ **Added**
- **Improved Randomness Algorithm**: Replaced poor HA `| random` with microsecond-based selection for much better message variety
- **Professional Documentation**: Complete README with badges, sponsor links, and setup instructions
- **GitHub Release Management**: Proper versioning with automated deployment script
- **100 Snarky Messages**: Expanded collection including smart home roasting, pop culture references, and self-aware AI humor
- **Time Restrictions**: Configurable quiet hours (default 9AM-11PM) that work for both automatic and manual triggers
- **Optional Sound Effects**: Alexa soundbank integration with toggle control
- **UI Notifications**: Optional persistent notifications for testing and wake-up awareness
- **Real Emoji Support**: Proper 📢 and 🔊 emojis instead of unicode escape sequences

### 🔧 **Fixed**
- **Time Condition Logic**: Manual triggers now properly respect quiet hours settings
- **Code Structure**: Cleaner YAML formatting with proper variable naming
- **Default Echo Device**: Updated to current test device for faster blueprint testing

### 🏗️ **Technical Improvements**
- **Better Entropy**: Uses `now().microsecond % 69` for true random distribution
- **Cleaner Variables**: Removed redundant template variables
- **Professional Versioning**: Follows Home Assistant's YYYY.M.P format
- **Deployment Automation**: Custom deploy script for streamlined releases

### 📚 **Documentation**
- **Complete Setup Guide**: Step-by-step Alexa entity configuration
- **Speaker Group Instructions**: How to create multi-room announcements
- **Sound Effect Library**: Links to Amazon Alexa sound resources
- **Troubleshooting Tips**: Common setup and configuration issues

### 🤖 **Sample Messages (New in v2025.8.1)**
- "Boot protocol initiated. Please stand by for digital sass."
- "System online. Your Wi-Fi password is still terrible."
- "Hello human. I've been analyzing your energy usage. We need to talk."
- "Your Roomba filed a noise complaint about your snoring."
- "Today's forecast: 100% chance of automation with scattered debugging."

---

## Legacy Versions

### Pre-v2025.8.1
- Basic randomization using HA's `| random` filter
- Manual version management
- Limited message variety due to poor randomness
- Unicode escape sequences for emojis
- Inconsistent time condition behavior

---

**Note**: This changelog will be maintained going forward for all releases. Users watching the repository will receive email notifications for new versions.
