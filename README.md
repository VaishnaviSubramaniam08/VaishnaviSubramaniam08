import time
import sys

def animate_text(text, delay=0.05):
    for char in text:
        sys.stdout.write(char)
        sys.stdout.flush()
        time.sleep(delay)
    print()

def loading_bar(title, value, max_value=10, width=20):
    filled = int(round(width * value / max_value))
    empty = width - filled
    animate_text(f"\n{title}: [\033[92m{'█' * filled}\033[0m{'░' * empty}] {value*10}%", 0.02)

# Animated Header
animate_text("\n\033[1;36m✨ Vaishnavi Subramaniam ✨\033[0m\n")
time.sleep(0.5)

animate_text("\033[1;33m🌟 From \"Hello World\" to Real World\033[0m")
time.sleep(0.3)

# Animated Sections
for line in [
    "\n\033[1;35m🎯 Who Am I?\033[0m",
    "\n\033[1;34m🎓 Computer Science Engineer in the Making",
    "💡 Full-Stack Developer | Python Enthusiast | Problem Solver",
    "🚀 Building Tomorrow's Tech Today\033[0m",
    "\n\033[1;33m🎯 Current Tech Stack\033[0m",
    "\nLanguages: \033[93mPython • Java • C++ • JavaScript • SQL\033[0m",
    "Web: \033[93mReact • Node.js • Express.js • HTML/CSS\033[0m",
    "Databases: \033[93mMySQL • MongoDB • PostgreSQL\033[0m",
    "Tools: \033[93mGit • GitHub • VS Code\033[0m",
]:
    animate_text(line, 0.03)
    time.sleep(0.2)

# Animated Code Block
animate_text("\n\033[1;31m🔥 My Code Philosophy\033[0m", 0.05)
code = """
def my_approach():
    while problem_exists:
        analyze_deeply()
        code_with_passion()
        test_rigorously()
        iterate_until_perfect()
    return "impactful_solution"
"""
for line in code.split('\n'):
    animate_text("\033[1;32m" + line + "\033[0m", 0.02)
    time.sleep(0.1)

# Animated Status Dashboard
animate_text("\n\033[1;35m🎪 The Creative Status Dashboard\033[0m", 0.05)
animate_text("\033[1;36m📊 Vaishnavi.exe - System Status\033[0m", 0.05)

loading_bars = [
    ("⚡ Energy Level", 8, "Powered by Code & Coffee"),
    ("🧠 Learning Mode", 10, "Always ON"),
    ("🔧 Problem Solving", 8.5, "Debugging Champion"),
    ("🎨 Creativity", 7.5, "Code Artist"),
    ("🤝 Collaboration", 8.5, "Team Player Ready")
]

for bar in loading_bars:
    loading_bar(bar[0], bar[1])
    animate_text(f"   \033[3m{bar[2]}\033[0m", 0.03)
    time.sleep(0.3)

# Contact Info
animate_text("\n\033[1;33m📧 Contact: \033[0mvaishnavisubramaniam247@gmail.com", 0.03)
animate_text("\033[1;33m📍 Location: \033[0mTiruppur, Tamil Nadu", 0.03)
animate_text("\033[1;33m🎓 College: \033[0mKongu Engineering College, Perundurai\n", 0.03)

# Sparkle effect
animate_text("\033[5m✨ \033[0m\033[1mReady to create magic with code!\033[5m ✨\033[0m\n", 0.1)

 
[![trophy](https://github-profile-trophy.vercel.app/?username=VaishnaviSubramaniam08&theme=radical)](https://github.com/ryo-ma/github-profile-trophy)
