# W02 - D04 - Drawing
***made by [Gabor](https://github.com/ed0wn)***

- [Drawing](#drawing)
    - [Line](#line)
    - [Rectangle](#rectangle)
    - [Polygon](#polygon)
    - [Oval](#oval)
    - [Color](#color)

## Drawing
### Line
```java
graphics.drawLine(x1, y1, x2, y2);
```

****

### Rectangle
```java
graphics.drawRect(x, y, WIDTH, HEIGHT);
```

****

### Polygon
```java
 	int[] xPoints;
 	int[] yPoints;
 	int nPoints; // number of angles
graphics.drawPolygon(xpoints, ypoints, npoints);
```

****

### Oval
```java
graphics.fillOval(x, y, WIDTH, HEIGHT);
```

****

### Color
```java
graphics.setColor(Color.BLACK);
graphics.setColor(new Color(R(0-255), G(0-255), B(0-255)));
```
