import math

# calculates 2d vector between points a = (x1, y1) and b = (x2, y2)
def two_d_vector_calculator(x1, y1, x2, y2):
    print('<', x2 - x1, ',', y2 - y1, '>')

# calculates 3d vector between points a = (x1, y1, z1) and b = (x2, y2, z2)
def three_d_vector_calculator(x1, y1, z1, x2, y2, z2):
    print('<', x2 - x1, ',', y2 - y1, ',', z2 - z1, '>')

#magnitude of 2 dimensional vector <x, y>
def two_d_magnitude(x, y):
    print(round(math.sqrt((x ** 2) + (y ** 2)), 3))

# magnitude of 3 dimensional vector <x, y, z>
def three_d_magnitude(x, y, z):
    print(round(math.sqrt((x ** 2) + (y ** 2) + (z ** 2)), 3))

# dot product of 2 dimensional vectors a = <a1, a2> and b = <b1, b2>
def two_d_dot_product(a1, a2, b1, b2):
    print(round((a1 * b1) + (a2 * b2), 3))

# dot product of 3 dimensional vectors a = <a1, a2, a3> and b = <b1, b2, b3>
def three_d_dot_product(a1, a2, a3, b1, b2, b3):
    print(round((a1 * b1) + (a2 * b2) + (a3 * b3), 3))

# angle between two vectors a = <a1, a2> and b = <b1, b2> in 2 dimensions
def two_d_angle_between_vectors(a1, a2, b1, b2):
    answer = float((a1 * b1) + (a2 * b2))
    magnitude_sum = math.sqrt((a1 ** 2) + (a2 ** 2)) * math.sqrt((b1 ** 2) + (b2 ** 2))
    print(round(((math.acos(answer / magnitude_sum)) * 180 / math.pi), 3))

# angle between two vectors a = <a1, a2, a3> and b = <b1, b2, b3> in 3 dimensions
def three_d_angle_between_vectors(a1, a2, a3, b1, b2, b3):
    answer = float((a1 * b1) + (a2 * b2) + (a3 * b3))
    magnitude_sum = math.sqrt((a1 ** 2) + (a2 ** 2) + (a3 ** 2)) * math.sqrt((b1 ** 2) + (b2 ** 2) + (b3 ** 2))
    print(round(((math.acos(answer / magnitude_sum)) * 180 / math.pi), 3))

# 2 dimensional scalar projection of vector b = <b1, b2> onto vector a = <a1, a2>
def two_d_scalar_projection(a1, a2, b1, b2):
    print(round(((a1 * b1) + (a2 * b2)) / (math.sqrt((a1 ** 2) + (a2 ** 2))), 3))

# 3 dimensional scalar projection of vector b = <b1, b2, b3> onto vector a = <a1, a2, a3>
def three_d_scalar_projection(a1, a2, a3, b1, b2, b3):
    print(round(((a1 * b1) + (a2 * b2) + (a3 * b3)) / (math.sqrt((a1 ** 2) + (a2 ** 2) + (a3 ** 2))), 3))

# 3 dimensional cross product between vectors a = <a1, a2, a3> and b = <b1, b2, b3>
def cross_product(a1, a2, a3, b1, b2, b3):
    x = round(((a2 * b3) - (a3 * b2)), 3)
    y = round(((a3 * b1) - (a1 * b3)), 3)
    z = round(((a1 * b2) - (a2 * b1)), 3)
    print('<', x, ',', y, ',', z, '>')
