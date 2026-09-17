print("🤖 Calculator AI Bot")
print("Type 'help' for commands")
print("Type 'bye' to exit")

while True:
    user = input("\nYou: ").strip().lower()

    if user == "hi" or user == "hello":
        print("Bot: Hello! 👋 I can calculate for you.")

    elif user == "help":
        print("Bot: Enter calculations like:")
        print("  5+3")
        print("  10-4")
        print("  6*7")
        print("  20/5")
        print("Type 'bye' to exit.")

    elif user == "bye":
        print("Bot: Goodbye! 👋")
        break

    else:
        try:
            answer = eval(user)
            print("Bot: Answer =", answer)
        except:
            print("Bot: I don't understand. Type 'help' for help.")
