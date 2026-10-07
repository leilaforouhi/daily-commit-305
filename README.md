def rotate_matrix(matrix):
    if not matrix:
        return []

    return [list(row) for row in zip(*matrix[::-1])]


if __name__ == "__main__":
    matrix = [
        [1, 2],
        [3, 4],
        [5, 6]
    ]

    print("Original:")
    for row in matrix:
        print(row)

    print("Rotated:")
    for row in rotate_matrix(matrix):
        print(row)
