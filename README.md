[perfect.py](https://github.com/user-attachments/files/27481551/perfect.py)
def is_perfect(n: int) -> bool:
    """���������� True, ���� ����� n �����������, ����� False."""
    if n <= 1:
        return False
    divisors_sum = 0
    for i in range(1, n // 2 + 1):
        if n % i == 0:
            divisors_sum += i
    return divisors_sum == n
