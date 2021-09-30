# testcode


list_of_numbers = [919, 234, 7777, 118]
# result = [19, 9, 10, 20]

result = [] #setting an empty list
for number in list_of_numbers: #iterating over the list
  total = 0 #setting a counter
  for str_number in str(number): #iterating over the individual number
    total += int(str_number) #setting a counter
    if total > 20: # condition
      total = 20 #re-setting a variable 
      break
  result.append(total) # adding the result to the empty list 
print(result)



# Iterate over the list en print the total of the numbers in each element, stop at 20. 

# for number in list_of_numbers:
#   i = 0
#   total = 0 
#   str_number = str(number)
#   while total <= 20 and i < len(str_number):
#       total += int(str_number[i])
#       i += 1
#   else:
#     if total > 20:
#       total = 20
#     print(total)

# def countElement(a):
#   g = {}
#   for i in a:
#     if i in g:
#       g[i] +=1
#     else:
#       g[i] =1
#   return g

# print(countElement(list_of_numbers))     
      

# my_list = [3, 5, 2, 1, 4, 4, 1]
# res = sum(1 for i in my_list if i % 2 != 0)
# print ("The number of odd elements: " + str(res))

# def countX(list, x):
#     count = 0
#     for ele in list:
#         if (ele == x):
#             count = count + 1
#     return count

# print(countX(koala_facts, "Joey"))

koala_facts = ["Joey", "fluffy", "climber", "bamboo", "cute", "pouch", "gray fur", "Crazy Joey"]

def get_koala_facts(list):
  new_list = [name for name in list if "Joey" in name]
  return new_list

print(get_koala_facts(koala_facts))


lst1=["Joe", "Sarah", "Mike", "Jess", "", "Matt", "", "Greg"]

def name_adder(list):
  i = 0 # setting a counter
  new_list = [] # setting up empty list 
  while i < len(list): # while loop
    if "Mike" != list[i]: #condition
      new_list.append(list[i]) # adding items to empty list 
    i = i + 1 # incrementing i, if you don't do this, it will be an infinite loop
  return new_list

print(name_adder(lst1))



lst=[10, 99, 98, 85, 45, 59, 65, 66, 76, 12, 35, 13, 100, 80, 95]



list2 = ["Sara", "Bego", "Teffa", "Sandra", "Paloma","Ginette", "Vero", "Elena", "Mechelle"]


  



list66 = ["Parijs", "Amsterdam", "Antananarivo", "Boekarest", "Seoul", "Seattle", "Washington", "Ho Chi Mihn Stad", "Tequicicalpa"]

def most_vowels(countries):
    new_list = []
    for name in countries:  # itereer over de lijst
        counter = 0  # counter
        for letter in name:  # itereer over elke letter

            if letter in "aeiouAEIOU":  # conditie
                counter += 1  # counter optellen

        new_list.append([name, counter])
    final_list = sorted(new_list, reverse=True,
                        key=lambda counter: counter[1])

    final_list = final_list[:3]

    final_list = sum(final_list, [])

    return final_list

print(most_vowels(list66))

def shortest_name(list_of_names):
  new_list = [min(list_of_names, key = len)]
  return new_list

print(shortest_name(list66))   

mylist = ["a", "b", "b", "c", "a"]
mylist = sorted(set(mylist))
print(mylist)


a_list = ["abcdefghijklmnopqrstuvwxyx"]
countries1 = ["Azerbaijan" , "Armenia", "Georgia" , "Russia", "Estonia", "Latvia", "Lithuania", "Finland",  "Sweden", "Denmark", "Iceland", "Poland", "Romania", "Bulgaria", "Greece", "Turkey", "Albania", "Serbia", "Czech", "Slovakia", "Croatia", "Bosnia", "Slovenia", "Austria", "Switzerland", "Italy", "Germany", "Holland", "France", "Belgium", "Spain","Portugal", "Luxembourg", "England", "Scotland", "Ireland", "Wales" , "Northern Ireland", "Macedonia", "Kosovo"]


