package machine;
import java.util.Scanner;

public class CoffeeMachine {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // state
        int remainingWater = 400;
        int remainingMilk = 540;
        int remainingBeans = 120;
        int remainingCups = 9;
        int remainingMoney = 550;

        // loop
        boolean programEnd = false;
        String action = "";
        while (!programEnd) {
            System.out.println("Write action (buy, fill, take, remaining, exit):");
            action = scanner.nextLine();
            switch (action) {
                case "exit":
                    programEnd = true;
                    break;
                case "remaining":
                    System.out.println("The coffee machine has:");
                    System.out.println(remainingWater + " ml of water");
                    System.out.println(remainingMilk + " ml of milk");
                    System.out.println(remainingBeans + " g of coffee beans");
                    System.out.println(remainingCups + " disposable cups");
                    System.out.println("$" + remainingMoney + " of money");
                    break;
                case "fill":
                    System.out.println("Write how many ml of water you want to add:");
                    remainingWater += scanner.nextInt();
                    System.out.println("Write how many ml of milk you want to add:");
                    remainingMilk += scanner.nextInt();
                    System.out.println("Write how many grams of coffee beans you want to add:");
                    remainingBeans += scanner.nextInt();
                    System.out.println("Write how many disposable cups of coffee you want to add:");
                    remainingCups += scanner.nextInt();
                    break;
                case "take":
                    System.out.printf("I gave you $%d%n", remainingMoney);
                    remainingMoney = 0;
                    break;
                case "buy":
                    System.out.println("What do you want to buy? 1 - espresso, 2 - latte, 3 - cappuccino, back - to main menu:");
                    String order = "";
                    order = scanner.nextLine();
                    if (order == "back") {
                        break;
                    }
                    if (order != "back") {
                        switch (order) {
                            case "1":
                                if (remainingWater >= 250) {
                                    if (remainingBeans >= 16) {
                                        if (remainingCups > 0) {
                                            System.out.println("I have enough resources, making you a coffee!");
                                            remainingWater -= 250;
                                            remainingBeans -= 16;
                                            remainingCups -= 1;
                                            remainingMoney += 4;
                                        } else {
                                            System.out.println("Sorry, not enough cups!");
                                        }
                                    } else {
                                        System.out.println("Sorry, not enough coffee beans!");
                                    }
                                } else {
                                    System.out.println("Sorry, not enough water!");
                                }
                                break;
                            case "2":
                                if (remainingWater >= 350) {
                                    if (remainingMilk >= 75) {
                                        if (remainingBeans >= 20) {
                                            if (remainingCups > 0) {
                                                System.out.println("I have enough resources, making you a coffee!");
                                                remainingWater -= 350;
                                                remainingMilk -= 75;
                                                remainingBeans -= 20;
                                                remainingCups -= 1;
                                                remainingMoney += 7;
                                            } else {
                                                System.out.println("Sorry, not enough cups!");
                                            }
                                        } else {
                                            System.out.println("Sorry, not enough coffee beans!");
                                        }
                                    } else {
                                        System.out.println("Sorry, not enough milk!");
                                    }
                                } else {
                                    System.out.println("Sorry, not enough water!");
                                }
                                break;
                            case "3":
                                if (remainingWater >= 200) {
                                    if (remainingMilk >= 100) {
                                        if (remainingBeans >= 12) {
                                            if (remainingCups > 0) {
                                                System.out.println("I have enough resources, making you a coffee!");
                                                remainingWater -= 200;
                                                remainingMilk -= 100;
                                                remainingBeans -= 12;
                                                remainingCups -= 1;
                                                remainingMoney += 6;
                                            } else {
                                                System.out.println("Sorry, not enough cups!");
                                            }
                                        } else {
                                            System.out.println("Sorry, not enough coffee beans!");
                                        }
                                    } else {
                                        System.out.println("Sorry, not enough milk!");
                                    }
                                } else {
                                    System.out.println("Sorry, not enough water!");
                                }
                                break;
                        }
                    break;
                    }
            }

        }
    }
}
