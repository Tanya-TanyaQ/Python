# Входные данные
weight = 80       # кг
height = 170      # см
age = 30          # примерный возраст
gender = 'male'   # или 'female'
activity_factor = 1.55  # умеренная активность (тренировки 3-5 дней в неделю)

# Формула Миффлина—Сан-Жеора:
if gender == 'male':
    bmr = 10 * weight + 6.25 * height - 5 * age + 5
else:
    bmr = 10 * weight + 6.25 * height - 5 * age - 161

# Расчёт суточной потребности:
calories = bmr * activity_factor

print(f"BMR: {bmr:.0f} ккал")
print(f"Суточная потребность (коллораж): {calories:.0f} ккал")
