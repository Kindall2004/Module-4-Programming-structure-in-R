# Module-4-Programming-structure-in-R
# Data vectors
Freq <- c(0.6, 0.3, 0.4, 0.4, 0.2, 0.6, 0.3, 0.4, 0.9, 0.2)
bloodp <- c(103, 87, 32, 42, 59, 109, 78, 205, 135, 176)
first <- c(1, 1, 1, 1, 0, 0, 0, 0, NA, 1)  # NA value present in the dataset
second <- c(0, 0, 1, 1, 0, 0, 1, 1, 1, 1)
finaldecision <- c(0, 1, 0, 1, 0, 1, 0, 1, 1, 1)

# Boxplot for Blood Pressure by First Doctor's Assessment
boxplot(bloodp ~ first, 
        main = "Boxplot of Blood Pressure by Doctor's First Assessment",
        xlab = "First Doctor's Assessment (0 = Good, 1 = Bad)",
        ylab = "Blood Pressure",
        col = c("lightblue", "lightgreen"))

# Histogram of Blood Pressure
hist(bloodp, 
     main = "Histogram of Blood Pressure", 
     xlab = "Blood Pressure", 
     col = "lightblue", 
     border = "black", 
     breaks = 10)
