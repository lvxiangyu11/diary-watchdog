🕰️ Diary Watchdog (Dead Man's Switch)
An automated digital safeguard monitoring my personal diary.

📖 About
This repository houses the "dead man's switch" script for my digital legacy. It is a standalone watchdog designed to continuously monitor my journaling activity in a separate, private diary repository.

If this system detects no updates or heartbeat signals in that private diary for 180 consecutive days, it will assume that I have passed away or encountered a severe, life-altering emergency. Upon reaching this critical threshold, this watchdog will automatically change the target diary repository's visibility from Private to Public and mark it as Archived.

⚙️ How It Works
Target Monitoring: A scheduled script periodically checks the latest commit history or modification timestamp of my private diary repository via API.

The 180-Day Countdown: The system maintains a strict 180-day timer. Any new update in the diary repo instantly resets this countdown to zero.

The Trigger Protocol: If the timer reaches exactly 180 days without any interruption, the failsafe is activated.

Final Action: The watchdog executes its final directive, using predefined tokens to publish the target diary repository, releasing my unfiltered thoughts and final footprint to the world as a read-only archive.

⚠️ Note to Visitors
You are currently viewing the open-source watchdog repository. Reading this README simply means you have found my automated safeguard system—my actual diary remains completely private and hidden. If you are ever able to access the separate diary repository, it means the 180-day failsafe has been triggered and I am no longer able to maintain it.
