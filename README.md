import math

#magnitude of 2 dimensional vector <x, y>
def two_d_magnitude(x, y):
    print(round(math.sqrt((x ** 2) + (y ** 2)), 2))

# magnitude of 3 dimensional vector <x, y, z>
def three_d_magnitude(x, y, z):
    print(round(math.sqrt((x ** 2) + (y ** 2) + (z ** 2)), 2))

# dot product of 2 dimensional vectors a = <a1, a2> and b = <b1, b2>
def two_d_dot_product(a1, a2, b1, b2):
    print(round((a1 * b1) + (a2 * b2), 2))

# dot product of 3 dimensional vectors a = <a1, a2, a3> and b = <b1, b2, b3>
def three_d_dot_product(a1, a2, a3, b1, b2, b3):
    print(round((a1 * b1) + (a2 * b2) + (a3 * b3), 2))

# angle between two vectors a = <a1, a2> and b = <b1, b2> in 2 dimensions
def two_d_angle_between_vectors(a1, a2, b1, b2):
    answer = float((a1 * b1) + (a2 * b2))
    magnitude_sum = math.sqrt((a1 ** 2) + (a2 ** 2)) * math.sqrt((b1 ** 2) + (b2 ** 2))
    print(round(((math.acos(answer / magnitude_sum)) * 180 / math.pi), 2))

# angle between two vectors a = <a1, a2, a3> and b = <b1, b2, b3> in 3 dimensions
def three_d_angle_between_vectors(a1, a2, a3, b1, b2, b3):
    answer = float((a1 * b1) + (a2 * b2) + (a3 * b3))
    magnitude_sum = math.sqrt((a1 ** 2) + (a2 ** 2) + (a3 ** 2)) * math.sqrt((b1 ** 2) + (b2 ** 2) + (b3 ** 2))
    print(round(((math.acos(answer / magnitude_sum)) * 180 / math.pi), 2))

# 2 dimensional scalar projection of vector b = <b1, b2> onto vector a = <a1, a2>
def two_d_scalar_projection(a1, a2, b1, b2):
    print(round(((a1 * b1) + (a2 * b2)) / (math.sqrt((a1 ** 2) + (a2 ** 2))), 2))

# 3 dimensional scalar projection of vector b = <b1, b2, b3> onto vector a = <a1, a2, a3>
def three_d_scalar_projection(a1, a2, a3, b1, b2, b3):
    print(round(((a1 * b1) + (a2 * b2) + (a3 * b3)) / (math.sqrt((a1 ** 2) + (a2 ** 2) + (a3 ** 2))), 2))

# 3 dimensional cross product between vectors a = <a1, a2, a3> and b = <b1, b2, b3>
def cross_product(a1, a2, a3, b1, b2, b3):
    print('<', ((a2 * b3) - (a3 * b2)), ',',  ((a3 * b1) - (a1 * b3)), ',', ((a1 * b2) - (a2 * b1)), '>')
