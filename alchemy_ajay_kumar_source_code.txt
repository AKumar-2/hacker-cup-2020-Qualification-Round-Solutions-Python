#input for no of cases
T = int(input())
for i in range (1, T+1):
    #input for shards and their arrangements
    no_of_shards = int(input())
    shards_arrangement = input()
    
    #Putting a counter
    count = 0
    for j in shards_arrangement:
        if j == "A":
            count += 1
        else:
            count -= 1
    if count == 1 or count == -1:
        print(f"Case #{i}: Y")
    else:
        print(f"Case #{i}: N")
