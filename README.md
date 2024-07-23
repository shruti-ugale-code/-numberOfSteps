# 🚀 Number of Steps to Reduce a Number to Zero

Welcome to the **Number of Steps to Reduce a Number to Zero** project! This repository contains a Java program that calculates the number of steps required to reduce a given number to zero. The steps involve either dividing the number by 2 if it's even or subtracting 1 if it's odd.

## 📋 Table of Contents

- [📖 Description](#-description)
- [✨ Features](#-features)
- [🛠️ Installation](#%EF%B8%8F-installation)
- [🚀 Usage](#-usage)
- [💻 Code](#-code)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

## 📖 Description

This project showcases a fundamental algorithmic problem: reducing a number to zero by repeatedly performing specified operations. The provided Java program uses a recursive approach to count the number of steps required to achieve this.

## ✨ Features

- 🔄 **Recursive Algorithm:** Utilizes recursion to solve the problem efficiently.
- 📚 **Educational:** Ideal for beginners to learn about recursion and conditional operations.
- 🧩 **Clear and Concise:** Straightforward implementation and easy to understand.

## 🛠️ Installation

To get started with this project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/numberOfStep.git
public class numberOfStep {
    public static void main(String[] args) {
        System.out.println(numberOfSteps(14));
    }

    public static int numberOfSteps(int num) {
        return helper(num, 0);
    }

    public static int helper(int n, int c) {
        if (n == 0) {
            return c;
        }
        if (n % 2 == 0) {
            return helper(n / 2, c + 1);
        }
        return helper(n - 1, c + 1);
    }
}
