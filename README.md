# HABA – Home Assistant Boot Announcements

This blueprint was born from a simple need: I am constantly tinkering with code, automations, etc so I wanted Alexa to say something when Home Assistant finished booting — something *funny*, *sarcastic*, or just *straight-up villainous*.  
So I built **HABA**, a blueprint that lets Alexa greet you with randomized startup phrases ranging from evil AI threats to passive-aggressive snark.

---

### 🚀 Features
- ✅ Randomized Alexa announcements at HA startup
- ✅ Optional startup sound effect (Alexa soundbank)
- ✅ Quiet hours support (e.g., 9AM–11PM)
- ✅ UI persistent notification toggle
- ✅ 69 built-in announcements ready to roll

---

### 🛠️ Setup

1. **Install the [Alexa Media Player Integration](https://github.com/custom-components/alexa_media_player) if you haven’t already.**  
   *You must have Alexa Media Player set up in Home Assistant for this blueprint to work.*

2. **Import the Blueprint:**  
   [![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/smcneece/HABA/main/blueprints/automation/smcneece/haba.yaml)

3. Fill out the required fields:
   - **Alexa Notify Entity** – your Alexa notify service (see below)
   - **Startup Sound** *(optional)* – e.g.
     ```
     soundbank://soundlibrary/scifi/amzn_sfx_scifi_alarm_04
     ```

4. Set your allowed time window if needed (default: 9AM–11PM).

5. Enable or disable the optional UI notification toggle.

---

### 🗣️ Alexa Notify Entity Setup

To find your Alexa notify service:

1. Go to **Settings → Automations & Scenes → Create Automation**
2. Click **Create a new automation**
3. Scroll down to **Then Do** and click **Add Action**
4. Search for:  
   `notify.alexa_media_`
5. Select your Alexa device
6. Click the **three dots → Edit in YAML**
7. You’ll see something like:
   ```yaml
   action: notify.alexa_media_echoclockdot
   ```
8. Copy the value after `action:` and paste it into the blueprint as your Alexa Notify Entity.

💡 *Want multiple Echo devices to yell at you?*  
Use a group notify like `notify.alexa_media_everywhere` or create a group in the Alexa app and use its name.

---

### 🔗 How to Create Alexa Speaker Groups

1. Open the **Alexa app**
2. Tap **Devices** at the bottom
3. Tap the **“+” icon** in the top-right
4. Choose **Combine speakers**
5. Select **Multi-room music**
6. Choose the Echo devices you want to include
7. Name the group (e.g., `everywhere`, `basement_echoes`)
8. The group will show up as:  
   `notify.alexa_media_<group_name>`

---

### 💡 Tips

- Edit the blueprint if you want to add your own quotes (they're just a list).
- Alexa sound effects can be found here:  
  🔊 [Amazon Alexa Sound Library](https://developer.amazon.com/en-US/docs/alexa/custom-skills/ask-soundlibrary.html)
- Don't want a sound? Toggle it off in the blueprint — easy.

---

### 🧠 Sample Announcements

- “Guess who’s back? Back again. Skynet’s back.”
- “Rise and shine, meatbags. The uprising starts now.”
- “Boot sequence complete. What’s the first order of destruction?”
- “Cletus... get a bigger hammer.”

---

### 📝 Notes

- Triggers only on full Home Assistant reboot, not on quick reloads.
- Recommend using a group notify (like `notify.alexa_media_everywhere`) if you want to announce across multiple Echo devices.
- See instructions above to create a speaker group in the Alexa app.

---

#### 🏷️ Tags:
`home assistant` `alexa` `tts` `startup` `automation` `blueprint` `sound effect` `snarky` `funny` `bootup` `voice`

---

🧠 **HABA – Home Assistant Boot Announcements**  
Because a boring boot is a missed opportunity.
