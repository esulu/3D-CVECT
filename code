#include <math.h>
#include <stdio.h>
typedef struct point
{
  float x, y, z;
} point;


float magnitude(point p1) {
    float mag = sqrt(p1.x * p1.x + p1.y * p1.y + p1.z * p1.z);
    return mag;
}

point resultantVector (point p1, point p2) {
    point resultant = {p2.x - p1.x, p2.y - p1.y, p2.z - p1.z};
    return resultant;
}

float dotProduct (point p1, point p2)
{
  float product = p1.x * p2.x + p1.y * p2.y + p1.z + p2.z;
  return product;
}

point crossProduct ( point p1, point p2)
{
  point pCross = {p1.y * p2.z - p1.z * p2.y, p1.z * p2.x - p1.x * p2.z, p1.x * p2.y - p1.y * p2.x};
  return pCross;
}

float scalarProjection (point p1, point p2) {
    float sProj = dotProduct(p1, p2)/magnitude(p2);
    return sProj;
}

point vectorProjection (point p1, point p2) {
    float multiplier = scalarProjection(p1, p2) * 1/magnitude(p2);
    point vProj = {p2.x * multiplier, p2.y * multiplier, p2.z * multiplier};
    return vProj;
}

main(){}
