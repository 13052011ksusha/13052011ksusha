def count_ways(distance): 
if distance == 0: 
return 1 
total_ways = 0 
for i in range(1, min(distance, 7) + 1): 
total_ways += count_ways(distance - i) 
return total_ways 

distance = 18 
total_ways = count_ways(distance) 
print(total_ways)
