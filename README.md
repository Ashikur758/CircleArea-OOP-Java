import java.util.Scanner;

class Circle {
    private double radius;

    Circle(double radius) {
        this.radius = radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }

    public double getRadius() {
        return radius;
    }

    public double calculateArea() {
        return Math.PI * radius * radius;
    }
}

public class CircleAreaOOP {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double r = sc.nextDouble();
        Circle c = new Circle(r);

        System.out.println(c.getRadius());
        System.out.println(c.calculateArea());

        sc.close();
    }
}
