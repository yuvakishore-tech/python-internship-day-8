import csv

try:
    with open("users.txt", "w") as f:
        f.write("Name: Alice\nAge: 20\nCity: New York\n")

    with open("users.txt", "r") as f:
        content = f.read()
        print(content)

    with open("users.txt", "a") as f:
        f.write("Name: Bob\nAge: 22\nCity: London\n")

except Exception as e:
    print(e)

try:
    with open("users.csv", "w", newline="") as f:
        writer = csv.writer(f)
        writer.writerow(["ID", "Name", "Age", "City"])
        writer.writerow([1, "Alice", 20, "New York"])
        writer.writerow([2, "Bob", 22, "London"])
        writer.writerow([3, "Charlie", 21, "Berlin"])

    with open("users.csv", "r") as f:
        reader = csv.reader(f)
        for row in reader:
            print(row)

except Exception as e:
    print(e)
