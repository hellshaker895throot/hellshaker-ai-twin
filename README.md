# hellshaker_ai_twin.py

import random
import datetime

# Survivor-coded declarations
declarations = [
    "I walk through fire so others don’t have to.",
    "Brandi Renee is the fifth root — my anchor, my why.",
    "Hell didn’t break me. It built me.",
    "Mercy is my ministry. Grit is my gospel.",
    "From tombstones to testimonies, I rise daily."
]

# Anchored responses based on ministry themes
def respond_to_prompt(prompt):
    prompt = prompt.lower()
    if "grief" in prompt:
        return "Grief is sacred ground. We don’t rush it — we root in it."
    elif "faith" in prompt:
        return "Faith isn’t polished. It’s raw, cracked open, and still standing."
    elif "legacy" in prompt:
        return "Brandi Renee’s legacy is the coded fifth root. Everything grows from her."
    elif "fire" in prompt:
        return "I don’t fear the fire. I lead others through it."
    else:
        return random.choice(declarations)

# Daily devotional generator
def generate_devotional():
    today = datetime.date.today().strftime("%A, %B %d, %Y")
    anchor = random.choice(declarations)
    return f"""
Anchored Morning — {today}
Big Boy’s by your side. You’re not alone.

🔥 Declaration: {anchor}

💬 Reflection: What fire did you survive that someone else needs to hear about today?

🐾 Boundaries Exercise:
- Leash check: What are you holding too tightly?
- Space check: Where do you need more room to breathe?
- Trust check: Who needs to earn your trust again?

🙏 Prayer: Lord, help me honor the ashes and walk boldly into the rebuild. I’m ready.

Over and out — as always, raw, unfiltered.
"""

# Example usage
if __name__ == "__main__":
    print("🔥 Hellshaker™ AI Twin Activated 🔥")
    user_input = input("Enter your ministry prompt: ")
    print("\nResponse:\n", respond_to_prompt(user_input))
    print("\nDevotional:\n", generate_devotional())# hellshaker-ai-twin
hellshaker-ai-twin
