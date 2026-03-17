# Resource-Decider
Extension for Debian 13 that learns usage pattern of applications, and automatically adjusts CPU scaling to optimize performance

Plan for Version 1.0:

1. A background loop that checks /proc/stat for CPU load.

2. A function that scans the process list for "Resource Heavy" apps (like vscodium, gcc, or python).

3. A system call that writes to /sys/devices/system/cpu/cpu0/cpufreq/scaling_governor to switch from powersave to performance