numbers = set()
for a in range(1, 8):
    for b in range(1, 8):
        for c in range(1, 8):
            if a + b + c < 8:
                continue
            numbers.add(f"{a}{b}{c}")
print(len(numbers))
