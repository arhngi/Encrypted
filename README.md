while True:
    print("\n\t1)Encrypted\n\t","2)Decrypted\n\t","3)Exit\n\t")
    choice = input("choice your option:")
    if choice == "1":
        plain_text = input("text: ")
        encrypted_text = ""
        for c in plain_text:
            x = ord(c) * 856 +100
            encrypted_text+=chr(x)
        print("encrypted_text",encrypted_text)

    elif choice == "2":
        encrypted_text = input("encrypted_text:")
        plain_text = ""
        for c in encrypted_text:
            x =(ord(c)-100) // 856
            plain_text += chr(x)
        print("plain_text",plain_text) 
        print()

    elif choice == "3":
        print("GoodBoy!")
        break
    else:
        print("Choice Is Wrong!")

