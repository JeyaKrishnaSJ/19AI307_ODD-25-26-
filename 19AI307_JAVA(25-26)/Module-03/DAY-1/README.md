# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
A jewelry store tracks gold rates for different types of customers. The base class is Customer with attributes like customerId, name, and purchaseWeight (in grams). There are two types of customers: RegularCustomer and PremiumCustomer. RegularCustomer gets a fixed discount of 2% on the gold rate per gram. PremiumCustomer gets a 5% discount plus a special cashback. The base gold rate per gram is input at runtime. For each customer, calculate the final price they pay:
finalPrice = purchaseWeight * (goldRatePerGram - discount)
For PremiumCustomer, additionally show cashback amount (which is 1% of the final price).

## AIM:
To Program to implement a Inheritance and Aggregation using Java

## ALGORITHM :
1.	Start the program.
2.	Read input values: customer type (Regular/Premium), customer ID, name, purchase weight, and gold rate per gram.
3.	Create the appropriate object (RegularCustomer or PremiumCustomer) based on the customer type using inheritance.
4.	Apply discount by overriding getDiscountRate() in each subclass and calculate the final price.
5.	For premium customers, additionally compute cashback (1% of final price).
6.	Display all details (ID, name, type, weight, rate, discount, final price, and cashback if applicable).

## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.*;
import java.text.DecimalFormat;

class Customer {
    String customerId, name;
    double purchaseWeight, goldRatePerGram;

    Customer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        this.customerId = customerId;
        this.name = name;
        this.purchaseWeight = purchaseWeight;
        this.goldRatePerGram = goldRatePerGram;
    }

    double getDiscountRate() {
        return 0;
    }

    double calculateFinalPrice() {
        double discountAmount = goldRatePerGram * getDiscountRate() / 100;
        double effectiveRate = goldRatePerGram - discountAmount;
        return purchaseWeight * effectiveRate;
    }

    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: General");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + (int)getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
    }
}

class RegularCustomer extends Customer {
    RegularCustomer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        super(customerId, name, purchaseWeight, goldRatePerGram);
    }

    double getDiscountRate() {
        return 2;
    }

    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: Regular");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + (int)getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
    }
}

class PremiumCustomer extends Customer {
    PremiumCustomer(String customerId, String name, double purchaseWeight, double goldRatePerGram) {
        super(customerId, name, purchaseWeight, goldRatePerGram);
    }

    double getDiscountRate() {
        return 5;
    }

    double getCashback() {
        return calculateFinalPrice() * 0.01;
    }

    void display() {
        DecimalFormat df = new DecimalFormat("0.00");
        System.out.println("Customer ID: " + customerId);
        System.out.println("Name: " + name);
        System.out.println("Customer Type: Premium");
        System.out.println("Purchase Weight: " + purchaseWeight + " grams");
        System.out.println("Gold Rate per Gram: " + goldRatePerGram);
        System.out.println("Discount: " + (int)getDiscountRate() + "%");
        System.out.println("Final Price: " + df.format(calculateFinalPrice()));
        System.out.println("Cashback: " + df.format(getCashback()));
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String type = sc.next();         // Regular or Premium
        String id = sc.next();           // customerId
        String name = sc.next();         // name
        double weight = sc.nextDouble(); // purchaseWeight
        double rate = sc.nextDouble();   // goldRatePerGram

        Customer c;
        if (type.equalsIgnoreCase("Regular")) {
            c = new RegularCustomer(id, name, weight, rate);
        } else {
            c = new PremiumCustomer(id, name, weight, rate);
        }

        c.display();
        sc.close();
    }
}

```

## OUTPUT:
<img width="1287" height="840" alt="Screenshot 2025-11-23 085524" src="https://github.com/user-attachments/assets/2b5abd4b-5ab9-40ca-bab8-56edbd3821c2" />



## RESULT:
Program to implement a Inheritance and Aggregation using Java is executed
