# PalindroneCheckerApp
BEGIN PalindromeCheckerApp

    DISPLAY "Enter a word or sentence:"
    INPUT userInput

    // Step 1: Normalize input
    CONVERT userInput to lowercase
    REMOVE all spaces from userInput

    // Step 2: Reverse the string
    SET reversedString = empty string

    FOR each character in userInput from last index to first index
        ADD character to reversedString
    END FOR

    // Step 3: Compare original and reversed
    IF userInput EQUALS reversedString THEN
        DISPLAY "It is a Palindrome"
    ELSE
        DISPLAY "It is NOT a Palindrome"
    END IF

END PalindromeCheckerApp