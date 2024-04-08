# JAVA OOP
### Date: 4/8/24
## Key Concepts

* Beginning of Class
     * Continuation of object-oriented programming
     * 4 HW Assignments this quarter
* Recap of Homework 1
     * Commit is making spaced changes to your code and prior to pushing it to your github
     * Pushing is actually putting your code on your repository on github
     * Cannot return two values in Java
     * Return complex type (an object that can return multiple results) - return type

## Code Snippets
Homework 1: Problem 4 answer (damn)
```java

package Problem4;

public class MillionDollarMaker {
    static final int MONTHS_PER_YEAR = 12;   // what does "final" do?

    // Do not change signature (function name, parameters, return type)
    public static CompoundingResult calculate(float initDeposit,
                                              float monthlyContribution,
                                              int lengthInYear,
                                              float rateInPercentage) {

        CompoundingResult result = new CompoundingResult(); // which constructor does this call?

        if (initDeposit <= 0 ||
                monthlyContribution <= 0 ||
                lengthInYear <= 0 ||
                rateInPercentage > 100 ||
                rateInPercentage < -100) {
            return result;
        }

        float yearlyContribution = monthlyContribution * MONTHS_PER_YEAR;   // why the constant MONTHS_PER_YEAR

        float accumulated = initDeposit;

        for (int i = 0; i < lengthInYear; i++) {
            accumulated = accumulated * (1 + rateInPercentage / 100.0f) + yearlyContribution;
        }

        result.setInvested(initDeposit + yearlyContribution * lengthInYear);
        result.setAccumulated(accumulated);

        return result;
    }
}

```

## Questions (Things I didn't understand)
* Why Problem 4 was wrong in my code
     * Find out after class (or if I even feel like it) 

## TODOs
- [ ] Read textbook
- [ ] Quiz 3
- [ ] Homework 2 (Start early)
