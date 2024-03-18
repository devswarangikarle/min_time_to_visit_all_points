# min_time_to_visit_all_points
Newton has three points, X, Y, and Z, positioned along a road. The time required to travel from X to Y or Y to X is denoted as A hours. Similarly, the time needed to travel between Y and Z, or Z and Y, is given as B hours. Additionally, the time required to travel from X to Z or Z to X is represented by C hours.

def min_time_to_visit_all_points(A, B, C):
    route1 = A + B
    route2 = B + C
    route3 = A + C
    min_time = min(route1, route2, route3)

    return min_time
A, B, C = map(int, input().split())

print(min_time_to_visit_all_points(A, B, C))
