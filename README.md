# sait
def is_prime(num):
    if num <= 1:
        return False
    c = 0
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            c += 1
    return c < 2


print([i for i in range(1000) if is_prime(i) == True])
