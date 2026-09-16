def count_numbers_by_sign(numbers):
    positive = sum(1 for number in numbers if number > 0)
    negative = sum(1 for number in numbers if number < 0)
    zero = numbers.count(0)

    return positive, negative, zero


if __name__ == "__main__":
    values = [5, -2, 0, 8, -7, 3, 0, -1]

    positive, negative, zero = count_numbers_by_sign(values)

    print("Values:", values)
    print("Positive:", positive)
    print("Negative:", negative)
    print("Zero:", zero)
