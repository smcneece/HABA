# HABA – Home Assistant Boot Announcements

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://raw.githubusercontent.com/smcneece/HABA/main/blueprints/automation/smcneece/haba.yaml)




This blueprint was born from a simple need: I wanted Alexa to say something when Home Assistant finished booting — something *funny*, *sarcastic*, or just *straight-up villainous*. So I built **HABA**, a blueprint that lets Alexa greet you with randomized startup phrases ranging from evil AI threats to passive-aggressive snark.

---

### 🚀 Features
- ✅ Randomized Alexa announcements at HA startup
- ✅ Optional sound effect using Alexa’s soundbank
- ✅ Quiet hours support (e.g., 9AM–11PM only)
- ✅ UI notification toggle (on/off)
- ✅ No helpers or input_booleans required
- ✅ Ready for GitHub import

---

### 🛠️ Setup

1. Click the **Import Blueprint** button above, or paste this into your browser:
   ```
   ```

2. Fill out the required fields:
   - **Alexa Notify Entity** – e.g. `notify.alexa_media_echo_dot`
   - **Startup Sound** *(optional)* – e.g.  
     ```
     soundbank://soundlibrary/scifi/amzn_sfx_scifi_alarm_04
     ```

3. Set your allowed time range if desired (default: 9AM–11PM).
4. Enable or disable the optional UI persistent notification.

---

### 💡 Tips

- Edit the blueprint to add your own quotes (they’re just in a list).
- Alexa sound effects can be found here:  
  🔊 [Amazon Alexa Sound Library](https://developer.amazon.com/en-US/docs/alexa/custom-skills/ask-soundlibrary.html)
- You don’t *have* to use a sound — just leave the field blank and she’ll speak the quote only.

---

### 🧠 Sample Announcements

- “Guess who’s back? Back again. Skynet’s back.”
- “Rise and shine, meatbags. The uprising starts now.”
- “Boot sequence complete. What’s the first order of destruction?”
- “Cletus... get a bigger hammer.”

---

### 📝 Notes

- This triggers only when Home Assistant fully restarts (not on core reload).
- If you run multiple Echo devices, use a group notify like `notify.alexa_media_everywhere` to reach them all.
- All text and sounds are optional — just delete the soundbank line if you want voice only.

---

#### 🏷️ Tags:
`home assistant` `alexa` `tts` `startup` `automation` `blueprint` `sound effect` `snarky` `funny` `bootup` `voice`

---

🧠 **HABA – Home Assistant Boot Announcements**  
Because a boring boot is a missed opportunity.
