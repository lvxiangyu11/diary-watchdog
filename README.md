🕰️ Diary Watchdog (Dead Man's Switch)
A digital safeguard and automated legacy trigger for my personal diary.

📖 About
This repository acts as an automated "dead man's switch" for my private diary. Its primary function is to continuously monitor my journaling activity. If the system detects no updates or heartbeat signals for 180 consecutive days, it will assume that I have either passed away or encountered a severe, life-altering emergency.

Upon reaching this critical threshold, the watchdog will execute its final directive: automatically making my private diary Public and marking it as Archived, thereby releasing my digital legacy to the world.

⚙️ How It Works
Continuous Monitoring: A scheduled automated script (the watchdog) periodically checks the last modified timestamp or commit history of the diary repository.

The 180-Day Countdown: The system maintains a strict 180-day timer. Any new diary entry, commit, or manual heartbeat signal instantly resets this countdown to zero.

The Trigger Protocol: If the timer reaches exactly 180 days without any interruption or reset, the failsafe is activated.

Final Action: The script utilizes API tokens to automatically change the diary repository's visibility settings from Private to Public and locks it as a read-only Archive.

⚠️ To the Reader
If you are reading the contents of my published diary, it means this failsafe has been triggered and I am no longer able to maintain it. The archived records represent my unfiltered thoughts, experiences, and my final footprint in the digital world.
