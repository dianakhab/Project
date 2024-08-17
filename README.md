calls = 0
def count_calls ():
    global calls
    calls += 1
def string_info (string):
    lenght =  len(string)
    upper =  string.upper()
    lower = string.lower()
    count_calls()
    return (lenght, upper, lower)
def is_contains (string, list_to_search):
    string_lower = string.lower()
    count_calls()
    return string.lower() in(item.lower() for item in list_to_search)

print(string_info('Orange'))
print(string_info('Apple'))
print(is_contains('Cucumber', ['cucumber', 'CuCuMbEr', 'CucuMBER']))
print(is_contains('watermelon', ['melon', 'water']))
print(calls)



[module_3_1.txt](https://github.com/user-attachments/files/16644627/module_3_1.txt)
