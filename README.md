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
