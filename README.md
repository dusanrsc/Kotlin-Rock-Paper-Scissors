# My Old Kotlin-Rock-Paper-Scissors Program From Year Ago...

# Just Commited Now...

# Example Of The Code:
```kotlin
package com.infinitysoftware.rockpaperscissors

// Main Program Function (Program Entry Point).
fun main() {

    // Printing Choice Message.
    println("Enter: 'Rock', 'Paper' or 'Scissors'.")

    // Local Variables Section.
    val choiceList = listOf("Rock", "Paper", "Scissors")

    var cpuChoice = choiceList.random()
    var playerChoice = readln().capitalize()

    // Printing Each Player Choices!
    println("Player: ${playerChoice}, CPU: ${cpuChoice}")

    // Game Logic Section.
    // Game Logic For The CPU-s Choice 'Rock'.
    if (playerChoice == "Rock" && cpuChoice == "Rock") {
        println("Its Tie!")
    } else if (playerChoice == "Paper" && cpuChoice == "Rock") {
        println("Player Win!")
    } else if (playerChoice == "Scissors" && cpuChoice == "Rock") {
        println("CPU Win!")

    // Game Logic For The CPU-s Choice 'Paper'.
    } else if (playerChoice == "Rock" && cpuChoice == "Paper") {
        println("CPU Win!")
    } else if (playerChoice == "Paper" && cpuChoice == "Paper") {
        println("Its Tie!")
    } else if (playerChoice == "Scissors" && cpuChoice == "Paper") {
        println("Player Win!")

    // Game Logic For The CPU-s Choice 'Scissros'.
    } else if (playerChoice == "Rock" && cpuChoice == "Scissors") {
        println("Player Win!")
    } else if (playerChoice == "Paper" && cpuChoice == "Scissors") {
        println("CPU Win!")
    } else if (playerChoice == "Scissors" && cpuChoice == "Scissors") {
        println("Its Tie!")

    // Else Logic (Error Catcher).
    } else {

        // If Player Input Is Invalid Call Main Program Function Again (Run Program Again).
        main()
    }

    // Calling Main Program Function Again After Game Is Finished (Run Program Again).
    main()
}
```
