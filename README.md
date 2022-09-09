# mochikaPython

## 1. Convert Strings to Camel Case

Complete the method/function so that it converts dash/underscore delimited words into camel casing. The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case).

`def to_camel_case(text):
    text = text.replace('_','$')
    text = text.replace('-','$')
    split = text.split('$')
    
    if(text == ''):
        return text
    else:
        leng = len(split)
        cont = 1
        arr = []
        
        arr.append(split[0])
        while(cont < leng):
            arr.append(split[cont].capitalize())
            cont+=1
            
        return ''.join(arr)
    `
   
## 2. Take a ten minute walk

You live in the city of Cartesia where all roads are laid out in a perfect grid. You arrived ten minutes too early to an appointment, so you decided to take the opportunity to go for a short walk. The city provides its citizens with a Walk Generating App on their phones -- everytime you press the button it sends you an array of one-letter strings representing directions to walk (eg. ['n', 's', 'w', 'e']). You always walk only a single block for each letter (direction) and you know it takes you one minute to traverse one city block, so create a function that will return true if the walk the app gives you will take you exactly ten minutes (you don't want to be early or late!) and will, of course, return you to your starting point. Return false otherwise.

``
