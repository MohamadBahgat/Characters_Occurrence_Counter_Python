# This Program is designed to count character occurrences in a given word, phrase or sentence.

def count_char(word, char = ''):
    if word == '':
        print('The chosen word is empty')
    else:
        word = word.lower()
        if char == '':
            print('since you did not specify and enter any character to be counted, so here is the count of the occurrences of the all characters in your chosen word.')
            #count = 0
            output = {}
            for i in word:
                if i in output:
                    output[i] += 1
                else:
                    output[i] = 1
            print(output)
        else:
            char = char.lower()
            count = 0
            for i in word:
                if i == char:
                    count += 1
            print('The char {} has been found in this word {} {} times.'.format(char, word, count))
            
count_char('00000')
count_char('koootyy')
count_char('Mohamed Bahgat Salah', 'a')
count_char(''Mohamed Bahgat Salah', 's')
