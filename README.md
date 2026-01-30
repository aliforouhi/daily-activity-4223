# daily_update.p
import datetime
import random

print("Daily GitHub activity - Day 42")

today = datetime.date.today()

# Simulate daily water intake (ml) and analyze
intakes = [random.randint(150, 350) for _ in range(8)]  # 8 glasses
total_intake = sum(intakes)
average_intake = round(total_intake / len(intakes), 2)

print(f"Today's date: {today}")
print("Water intake per glass (ml):", intakes)
print("Total intake (ml):", total_intake)
print("Average per glass (ml):", average_intake)
print("Glasses above average:", len([i for i in intakes if i > average_intake]))
