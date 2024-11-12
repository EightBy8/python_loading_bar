import math
import colorama
#Adding Comment to line 3
colorama.init()

def progress_bar(progress, total, color=colorama.Fore.GREEN):
    percent = 100 * (progress / float(total))
    bar = '█' * int(percent) + '-' * (100 - int(percent))
    print(color + f"|{bar}| {percent:.2f}%", end="\r") 

numbers = [x * 5 for x in range(2000, 3000)]
results = []


progress_bar(0, len(numbers))
for i, x in enumerate(numbers):
    results.append(math.factorial(x))
    progress_bar(i + 1, len(numbers))

print(colorama.Style.RESET_ALL)

